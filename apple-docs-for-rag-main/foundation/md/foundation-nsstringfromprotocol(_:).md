

- Foundation
-  NSStringFromProtocol(\_:) 

Function

# NSStringFromProtocol(\_:)

Returns the name of a protocol as a string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSStringFromProtocol(_ proto: Protocol) -> String
```

## Parameters 

`proto`  

A protocol.

## Return Value

A string containing the name of `proto`.

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

func NSProtocolFromString(String) -> Protocol?

Returns a the protocol with a given name.

