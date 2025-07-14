

- Core Data
-  NSMergePolicyType 

Enumeration

# NSMergePolicyType

Constants that define merge policy types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum NSMergePolicyType
```

## Topics

### Policies

case errorMergePolicyType

The default merge policy for all managed object contexts.

case mergeByPropertyStoreTrumpMergePolicyType

A property-based merge policy that applies external changes.

case mergeByPropertyObjectTrumpMergePolicyType

A property-based merge policy that applies in-memory changes.

case overwriteMergePolicyType

A merge policy type that overwrites the entire stored object.

case rollbackMergePolicyType

A merge policy that discards unsaved changes.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Policies

var NSErrorMergePolicy: AnyObject

The default merge policy for all managed object contexts.

var NSMergeByPropertyStoreTrumpMergePolicy: AnyObject

A property-based merge policy that applies external changes.

var NSMergeByPropertyObjectTrumpMergePolicy: AnyObject

A property-based merge policy that applies in-memory changes.

var NSOverwriteMergePolicy: AnyObject

A merge policy that overwrites the entire stored object.

var NSRollbackMergePolicy: AnyObject

A merge policy that discards unsaved changes.

