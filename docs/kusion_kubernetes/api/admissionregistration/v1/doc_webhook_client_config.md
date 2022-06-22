# webhook_client_config

Source: [base/pkg/kusion_kubernetes/api/admissionregistration/v1/webhook_client_config.k](https://github.com/KusionStack/konfig/tree/main//base/pkg/kusion_kubernetes/api/admissionregistration/v1/webhook_client_config.k)

This is the webhook\_client\_config module in kusion\_kubernetes.api.admissionregistration.v1 package.<br />This file was generated by the KCL auto-gen tool. DO NOT EDIT.<br />Editing this file might prove futile when you re-run the KCL auto-gen generate command.

## Schema WebhookClientConfig

WebhookClientConfig contains the information to make a TLS connection with the webhook

### Attributes

|Name and Description|Type|Default Value|Required|
|--------------------|----|-------------|--------|
|**caBundle**<br />     `caBundle` is a PEM encoded CA bundle which will be used to validate the webhook's server certificate. If unspecified, system trust roots on the apiserver are used.<br />url : str, default is Undefined, optional<br />     `url` gives the location of the webhook, in standard URL form (`scheme://host:port/path`). Exactly one of `url` or `service` must be specified.|str|Undefined|optional|
|**url**|str|Undefined|optional|
|**service**|[ServiceReference](doc_service_reference.md#schema-servicereference)|Undefined|optional|
<!-- Auto generated by kcl-doc tool, please do not edit. -->