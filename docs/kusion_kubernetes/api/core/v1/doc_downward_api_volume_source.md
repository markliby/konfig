# downward_api_volume_source

Source: [base/pkg/kusion_kubernetes/api/core/v1/downward_api_volume_source.k](https://github.com/KusionStack/konfig/tree/main//base/pkg/kusion_kubernetes/api/core/v1/downward_api_volume_source.k)

This is the downward\_api\_volume\_source module in kusion\_kubernetes.api.core.v1 package.<br />This file was generated by the KCL auto-gen tool. DO NOT EDIT.<br />Editing this file might prove futile when you re-run the KCL auto-gen generate command.

## Schema DownwardAPIVolumeSource

DownwardAPIVolumeSource represents a volume containing downward API info. Downward API volumes support ownership management and SELinux relabeling.

### Attributes

|Name and Description|Type|Default Value|Required|
|--------------------|----|-------------|--------|
|**defaultMode**<br />Optional: mode bits to use on created files by default. Must be a Optional: mode bits used to set permissions on created files by default. Must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decimal values, JSON requires decimal values for mode bits. Defaults to 0644. Directories within the path are not affected by this setting. This might be in conflict with other options that affect the file mode, like fsGroup, and the result can be other mode bits set.|int|Undefined|optional|
|**items**<br />Items is a list of downward API volume file|[[v1.DownwardAPIVolumeFile](doc_downward_api_volume_file.md#schema-downwardapivolumefile)]|Undefined|optional|
<!-- Auto generated by kcl-doc tool, please do not edit. -->