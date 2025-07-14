

- Foundation
-  NSStringFromClass(\_:) 

Function

# NSStringFromClass(\_:)

Returns the name of a class as a string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSStringFromClass(_ aClass: AnyClass) -> String
```

## Parameters 

`aClass`  

A class.

## Return Value

A string containing the name of `aClass`. If `aClass` is `nil`, returns `nil`.

## See Also

### Type Lookup

func NSClassFromString(String) -> AnyClass?

Obtains a class by name.

func NSSelectorFromString(String) -> Selector

Returns the selector with a given name.

func NSStringFromSelector(Selector) -> String

Returns a string representation of a given selector.

func NSStringFromProtocol(Protocol) -> String

Returns the name of a protocol as a string.

func NSProtocolFromString(String) -> Protocol?

Returns a the protocol with a given name.

