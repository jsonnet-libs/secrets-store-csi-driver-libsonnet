---
permalink: /1.2/nogroup/v1alpha1/secretProviderClass/
---

# nogroup.v1alpha1.secretProviderClass

"SecretProviderClass is the Schema for the secretproviderclasses API"

## Index

* [`fn new(name, tenantId, keyvaultName, userAssignedIdentityId, objects='[]', secretName='null', secretObjects='[]')`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withParameters(parameters)`](#fn-specwithparameters)
  * [`fn withParametersMixin(parameters)`](#fn-specwithparametersmixin)
  * [`fn withProvider(provider)`](#fn-specwithprovider)
  * [`fn withSecretObjects(secretObjects)`](#fn-specwithsecretobjects)
  * [`fn withSecretObjectsMixin(secretObjects)`](#fn-specwithsecretobjectsmixin)
  * [`obj spec.parameters`](#obj-specparameters)
    * [`fn newAzureParameters(tenantId, keyvaultName, userAssignedIdentityId, useVMManagedIdentity='true', usePodIdentity='false')`](#fn-specparametersnewazureparameters)
    * [`fn withClientId(withClientId)`](#fn-specparameterswithclientid)
    * [`fn withCloudName(withCloudName)`](#fn-specparameterswithcloudname)
    * [`fn withKeyvaultName(withKeyvaultName)`](#fn-specparameterswithkeyvaultname)
    * [`fn withObjects(objects)`](#fn-specparameterswithobjects)
    * [`fn withTenantId(withTenantId)`](#fn-specparameterswithtenantid)
    * [`fn withUsePodIdentity(usePodIdentity)`](#fn-specparameterswithusepodidentity)
    * [`fn withUseVMManagedIdentity(withUseVMManagedIdentity)`](#fn-specparameterswithusevmmanagedidentity)
    * [`fn withUserAssignedIdentityId(withUserAssignedIdentityId)`](#fn-specparameterswithuserassignedidentityid)
  * [`obj spec.secretObjects`](#obj-specsecretobjects)
    * [`fn new(name, objects)`](#fn-specsecretobjectsnew)
    * [`fn withAnnotations(annotations)`](#fn-specsecretobjectswithannotations)
    * [`fn withAnnotationsMixin(annotations)`](#fn-specsecretobjectswithannotationsmixin)
    * [`fn withData(data)`](#fn-specsecretobjectswithdata)
    * [`fn withDataMixin(data)`](#fn-specsecretobjectswithdatamixin)
    * [`fn withLabels(labels)`](#fn-specsecretobjectswithlabels)
    * [`fn withLabelsMixin(labels)`](#fn-specsecretobjectswithlabelsmixin)
    * [`fn withSecretName(secretName)`](#fn-specsecretobjectswithsecretname)
    * [`fn withType(type)`](#fn-specsecretobjectswithtype)
    * [`obj spec.secretObjects.data`](#obj-specsecretobjectsdata)
      * [`fn new(key, object)`](#fn-specsecretobjectsdatanew)
      * [`fn withKey(key)`](#fn-specsecretobjectsdatawithkey)
      * [`fn withObjectName(objectName)`](#fn-specsecretobjectsdatawithobjectname)

## Fields

### fn new

```ts
new(name, tenantId, keyvaultName, userAssignedIdentityId, objects='[]', secretName='null', secretObjects='[]')
```

Create new azure specific secretProviderClass.

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"SecretProviderClassSpec defines the desired state of SecretProviderClass"

### fn spec.withParameters

```ts
withParameters(parameters)
```

"Configuration for specific provider"

### fn spec.withParametersMixin

```ts
withParametersMixin(parameters)
```

"Configuration for specific provider"

**Note:** This function appends passed data to existing values

### fn spec.withProvider

```ts
withProvider(provider)
```

"Configuration for provider name"

### fn spec.withSecretObjects

```ts
withSecretObjects(secretObjects)
```



### fn spec.withSecretObjectsMixin

```ts
withSecretObjectsMixin(secretObjects)
```



**Note:** This function appends passed data to existing values

## obj spec.parameters



### fn spec.parameters.newAzureParameters

```ts
newAzureParameters(tenantId, keyvaultName, userAssignedIdentityId, useVMManagedIdentity='true', usePodIdentity='false')
```

 shortcut to define new azure specific prameters with defaults

### fn spec.parameters.withClientId

```ts
withClientId(withClientId)
```

Helper-function to set attribute according to to specification (https://learn.microsoft.com/en-us/azure/aks/csi-secrets-store-identity-access#use-a-user-assigned-managed-identity)

### fn spec.parameters.withCloudName

```ts
withCloudName(withCloudName)
```

Helper-function to set attribute according to to specification (https://learn.microsoft.com/en-us/azure/aks/csi-secrets-store-identity-access#use-a-user-assigned-managed-identity)

### fn spec.parameters.withKeyvaultName

```ts
withKeyvaultName(withKeyvaultName)
```

Helper-function to set attribute according to to specification (https://learn.microsoft.com/en-us/azure/aks/csi-secrets-store-identity-access#use-a-user-assigned-managed-identity)

### fn spec.parameters.withObjects

```ts
withObjects(objects)
```

Function to render objects-text. Takes an object-array e.g. [{objectName:"name",objectType:"secret"}] or an single object.

### fn spec.parameters.withTenantId

```ts
withTenantId(withTenantId)
```

Helper-function to set attribute according to to specification (https://learn.microsoft.com/en-us/azure/aks/csi-secrets-store-identity-access#use-a-user-assigned-managed-identity)

### fn spec.parameters.withUsePodIdentity

```ts
withUsePodIdentity(usePodIdentity)
```

Helper-function to set attribute according to to specification (https://learn.microsoft.com/en-us/azure/aks/csi-secrets-store-identity-access#use-a-user-assigned-managed-identity)

### fn spec.parameters.withUseVMManagedIdentity

```ts
withUseVMManagedIdentity(withUseVMManagedIdentity)
```

Helper-function to set attribute according to to specification (https://learn.microsoft.com/en-us/azure/aks/csi-secrets-store-identity-access#use-a-user-assigned-managed-identity)

### fn spec.parameters.withUserAssignedIdentityId

```ts
withUserAssignedIdentityId(withUserAssignedIdentityId)
```

Helper-function to set attribute according to to specification (https://learn.microsoft.com/en-us/azure/aks/csi-secrets-store-identity-access#use-a-user-assigned-managed-identity)

## obj spec.secretObjects



### fn spec.secretObjects.new

```ts
new(name, objects)
```

Create new secretsObject.

### fn spec.secretObjects.withAnnotations

```ts
withAnnotations(annotations)
```

"annotations of k8s secret object"

### fn spec.secretObjects.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"annotations of k8s secret object"

**Note:** This function appends passed data to existing values

### fn spec.secretObjects.withData

```ts
withData(data)
```



### fn spec.secretObjects.withDataMixin

```ts
withDataMixin(data)
```



**Note:** This function appends passed data to existing values

### fn spec.secretObjects.withLabels

```ts
withLabels(labels)
```

"labels of K8s secret object"

### fn spec.secretObjects.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"labels of K8s secret object"

**Note:** This function appends passed data to existing values

### fn spec.secretObjects.withSecretName

```ts
withSecretName(secretName)
```

"name of the K8s secret object"

### fn spec.secretObjects.withType

```ts
withType(type)
```

"type of K8s secret object"

## obj spec.secretObjects.data



### fn spec.secretObjects.data.new

```ts
new(key, object)
```

Create new secretsObjects data entry. Object has to have an objectName field or should be provided as objectName string

### fn spec.secretObjects.data.withKey

```ts
withKey(key)
```

"data field to populate"

### fn spec.secretObjects.data.withObjectName

```ts
withObjectName(objectName)
```

"name of the object to sync"