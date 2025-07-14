

- Core Data
- NSMergePolicyType
-  NSMergePolicyType.errorMergePolicyType 

Case

# NSMergePolicyType.errorMergePolicyType

The default merge policy for all managed object contexts.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case errorMergePolicyType
```

## Discussion

If a save fails because of conflicting objects, you can find the IDs of those objects in error’s `userInfo` dictionary. Use the NSInsertedObjectsKey and NSUpdatedObjectsKey keys to extract the object IDs.

## See Also

### Policies

case mergeByPropertyStoreTrumpMergePolicyType

A property-based merge policy that applies external changes.

case mergeByPropertyObjectTrumpMergePolicyType

A property-based merge policy that applies in-memory changes.

case overwriteMergePolicyType

A merge policy type that overwrites the entire stored object.

case rollbackMergePolicyType

A merge policy that discards unsaved changes.

