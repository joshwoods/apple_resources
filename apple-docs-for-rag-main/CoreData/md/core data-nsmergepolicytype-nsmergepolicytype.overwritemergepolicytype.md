

- Core Data
- NSMergePolicyType
-  NSMergePolicyType.overwriteMergePolicyType 

Case

# NSMergePolicyType.overwriteMergePolicyType

A merge policy type that overwrites the entire stored object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case overwriteMergePolicyType
```

## Discussion

This policy merges conflicts between the persistent store’s version of the object and the current in-memory version by saving the entire in-memory object to the persistent store.

## See Also

### Policies

case errorMergePolicyType

The default merge policy for all managed object contexts.

case mergeByPropertyStoreTrumpMergePolicyType

A property-based merge policy that applies external changes.

case mergeByPropertyObjectTrumpMergePolicyType

A property-based merge policy that applies in-memory changes.

case rollbackMergePolicyType

A merge policy that discards unsaved changes.

