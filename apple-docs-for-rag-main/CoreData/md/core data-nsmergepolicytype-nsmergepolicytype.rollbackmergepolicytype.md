

- Core Data
- NSMergePolicyType
-  NSMergePolicyType.rollbackMergePolicyType 

Case

# NSMergePolicyType.rollbackMergePolicyType

A merge policy that discards unsaved changes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case rollbackMergePolicyType
```

## Discussion

This policy merges conflicts between the persistent store’s version of the object and the current in-memory version by discarding unsaved changes.

## See Also

### Policies

case errorMergePolicyType

The default merge policy for all managed object contexts.

case mergeByPropertyStoreTrumpMergePolicyType

A property-based merge policy that applies external changes.

case mergeByPropertyObjectTrumpMergePolicyType

A property-based merge policy that applies in-memory changes.

case overwriteMergePolicyType

A merge policy type that overwrites the entire stored object.

