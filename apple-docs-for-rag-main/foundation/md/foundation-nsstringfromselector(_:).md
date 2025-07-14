

- Foundation
-  NSStringFromSelector(\_:) 

Function

# NSStringFromSelector(\_:)

Returns a string representation of a given selector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSStringFromSelector(_ aSelector: Selector) -> String
```

## Parameters 

`aSelector`  

A selector.

## Return Value

A string representation of `aSelector`.

## See Also

### Type Lookup

func NSClassFromString(String) -> AnyClass?

Obtains a class by name.

func NSStringFromClass(AnyClass) -> String

Returns the name of a class as a string.

func NSSelectorFromString(String) -> Selector

Returns the selector with a given name.

func NSStringFromProtocol(Protocol) -> String

Returns the name of a protocol as a string.

func NSProtocolFromString(String) -> Protocol?

Returns a the protocol with a given name.

