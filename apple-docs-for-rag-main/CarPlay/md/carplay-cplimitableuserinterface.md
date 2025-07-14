

- CarPlay
-  CPLimitableUserInterface 

Structure

# CPLimitableUserInterface

The types of limitable user interface elements.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
struct CPLimitableUserInterface
```

## Topics

### User Interface Limits

static var keyboard: CPLimitableUserInterface

Indicates that the car is limiting the keyboard display.

static var lists: CPLimitableUserInterface

Indicates that the car is limiting the display of lists.

### Initializers

init(rawValue: UInt)

Initializes a limitable user interface element using the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting the Limits

var limitedUserInterfaces: CPLimitableUserInterface

A bit mask value that indicates the user interface limits.

