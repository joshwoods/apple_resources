

- Foundation
-  NSTextCheckingTypes 

Type Alias

# NSTextCheckingTypes

Defines the types of checking that are available. These values can be combined using the C-bitwise OR operator. The system supports its own internal types, and the user can extend those types by subclassing `NSTextCheckingResult` and adding their own custom types.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias NSTextCheckingTypes = UInt64
```

## Topics

### Constants

var NSTextCheckingAllSystemTypes: NSTextCheckingTypes

Checking types supported by the system. The first 32 types are reserved.

var NSTextCheckingAllCustomTypes: NSTextCheckingTypes

Checking types that can be used by clients.

var NSTextCheckingAllTypes: NSTextCheckingTypes

All possible checking types, both system- and user-supported.

## See Also

### Constants

Keys for Transit Components

The following constants identify the possible keys returned in the components dictionary.

Keys for Address Components

The following constants identify the possible keys returned in the addressComponents dictionary.

struct CheckingType

These constants specify the type of checking the methods should do. They are returned by resultType.

struct NSTextCheckingKey

Anonymous

