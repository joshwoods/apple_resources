

- Core Data
-  NSDeleteRule 

Enumeration

# NSDeleteRule

Constants that determine what happens when you delete a relationship’s owning managed object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum NSDeleteRule
```

## Topics

### Delete Rules

case noActionDeleteRule

A rule that prevents modification of the referenced managed objects.

case nullifyDeleteRule

A rule that nullifies the inverse relationship of the referenced managed objects.

case cascadeDeleteRule

A rule that deletes the referenced managed objects.

case denyDeleteRule

A rule that prevents the deletion of the owning managed object if the relationship has references to other objects.

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

### Configuring Delete Behavior

var deleteRule: NSDeleteRule

The rule to apply when you delete the relationship’s owning managed object.

