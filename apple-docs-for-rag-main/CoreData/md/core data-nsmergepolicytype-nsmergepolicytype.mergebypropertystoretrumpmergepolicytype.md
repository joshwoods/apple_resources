

- Core Data
- NSMergePolicyType
-  NSMergePolicyType.mergeByPropertyStoreTrumpMergePolicyType 

Case

# NSMergePolicyType.mergeByPropertyStoreTrumpMergePolicyType

A property-based merge policy that applies external changes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case mergeByPropertyStoreTrumpMergePolicyType
```

## Discussion

A policy that merges conflicts between the persistent store’s version of the object and the current in-memory version by individual property, with external changes trumping in-memory changes.

## See Also

### Policies

case errorMergePolicyType

The default merge policy for all managed object contexts.

case mergeByPropertyObjectTrumpMergePolicyType

A property-based merge policy that applies in-memory changes.

case overwriteMergePolicyType

A merge policy type that overwrites the entire stored object.

case rollbackMergePolicyType

A merge policy that discards unsaved changes.

