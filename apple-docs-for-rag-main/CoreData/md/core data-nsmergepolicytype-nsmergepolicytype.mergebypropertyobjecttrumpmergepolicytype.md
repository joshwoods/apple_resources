

- Core Data
- NSMergePolicyType
-  NSMergePolicyType.mergeByPropertyObjectTrumpMergePolicyType 

Case

# NSMergePolicyType.mergeByPropertyObjectTrumpMergePolicyType

A property-based merge policy that applies in-memory changes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case mergeByPropertyObjectTrumpMergePolicyType
```

## Mentioned in 

Configuring Entities

## Discussion

A policy that merges conflicts between the persistent store’s version of the object and the current in-memory version by individual property, with in-memory changes trumping external changes.

## See Also

### Policies

case errorMergePolicyType

The default merge policy for all managed object contexts.

case mergeByPropertyStoreTrumpMergePolicyType

A property-based merge policy that applies external changes.

case overwriteMergePolicyType

A merge policy type that overwrites the entire stored object.

case rollbackMergePolicyType

A merge policy that discards unsaved changes.

