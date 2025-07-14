

- Address Book
-  ABPeoplePickerSelectionBehavior 

Structure

# ABPeoplePickerSelectionBehavior

Constants indicating the possible value selection behaviors.

macOS

``` source
struct ABPeoplePickerSelectionBehavior
```

## Overview

These constants are of the type ABPeoplePickerSelectionBehavior and are used by valueSelectionBehavior.

## Topics

### Selection Behaviors

var ABNoValueSelection: ABPeoplePickerSelectionBehavior

The user cannot select individual values.

var ABSingleValueSelection: ABPeoplePickerSelectionBehavior

The user can select a single value.

var ABMultipleValueSelection: ABPeoplePickerSelectionBehavior

The user can select multiple values.

### Initializers

init(UInt32)

Initializes a constant from an integer value that represents a picker selection behavior.

init(rawValue: UInt32)

Initializes a constant from a raw value that represents a picker selection behavior.

### Instance Properties

var rawValue: UInt32

The raw integer value of a possible selection behavior constant.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying Selection Behavior

var valueSelectionBehavior: ABPeoplePickerSelectionBehavior

The current selection behavior.

