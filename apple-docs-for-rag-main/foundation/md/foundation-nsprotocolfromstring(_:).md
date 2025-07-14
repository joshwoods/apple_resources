

- Foundation
-  NSProtocolFromString(\_:) 

Function

# NSProtocolFromString(\_:)

Returns a the protocol with a given name.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSProtocolFromString(_ namestr: String) -> Protocol?
```

## Parameters 

`namestr`  

The name of a protocol.

## Return Value

The protocol object named by `namestr`, or `nil` if no protocol by that name is currently loaded. If `namestr` is `nil`, returns `nil`.

## See Also

### Type Lookup

func NSClassFromString(String) -> AnyClass?

Obtains a class by name.

func NSStringFromClass(AnyClass) -> String

Returns the name of a class as a string.

func NSSelectorFromString(String) -> Selector

Returns the selector with a given name.

func NSStringFromSelector(Selector) -> String

Returns a string representation of a given selector.

func NSStringFromProtocol(Protocol) -> String

Returns the name of a protocol as a string.

