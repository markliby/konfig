# policy_rule

Source: [base/pkg/kusion_kubernetes/api/rbac/v1/policy_rule.k](https://github.com/KusionStack/konfig/tree/main//base/pkg/kusion_kubernetes/api/rbac/v1/policy_rule.k)

This is the policy\_rule module in kusion\_kubernetes.api.rbac.v1 package.<br />This file was generated by the KCL auto-gen tool. DO NOT EDIT.<br />Editing this file might prove futile when you re-run the KCL auto-gen generate command.

## Schema PolicyRule

PolicyRule holds information that describes a policy rule, but does not contain information about who the rule applies to or which namespace the rule applies to.

### Attributes

|Name and Description|Type|Default Value|Required|
|--------------------|----|-------------|--------|
|**apiGroups**<br />APIGroups is the name of the APIGroup that contains the resources.  If multiple API groups are specified, any action requested against one of the enumerated resources in any API group will be allowed.|[str]|Undefined|optional|
|**nonResourceURLs**<br />NonResourceURLs is a set of partial urls that a user should have access to.  \*s are allowed, but only as the full, final step in the path Since non-resource URLs are not namespaced, this field is only applicable for ClusterRoles referenced from a ClusterRoleBinding. Rules can either apply to API resources (such as "pods" or "secrets") or non-resource URL paths (such as "/api"),  but not both.|[str]|Undefined|optional|
|**resourceNames**<br />ResourceNames is an optional white list of names that the rule applies to.  An empty set means that everything is allowed.|[str]|Undefined|optional|
|**resources**<br />Resources is a list of resources this rule applies to. '\*' represents all resources.|[str]|Undefined|optional|
|**verbs**<br />Verbs is a list of Verbs that apply to ALL the ResourceKinds and AttributeRestrictions contained in this rule. '\*' represents all verbs.|[str]|Undefined|**required**|
<!-- Auto generated by kcl-doc tool, please do not edit. -->