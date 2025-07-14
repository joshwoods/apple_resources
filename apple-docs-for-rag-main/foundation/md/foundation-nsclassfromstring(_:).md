

- Foundation
-  NSClassFromString(\_:) 

Function

# NSClassFromString(\_:)

Obtains a class by name.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSClassFromString(_ aClassName: String) -> AnyClass?
```

## Parameters 

`aClassName`  

The name of a class.

## Return Value

The class object named by `aClassName`, or `nil` if no class by that name is currently loaded. If `aClassName` is `nil`, returns `nil`.

## See Also

### Type Lookup

func NSStringFromClass(AnyClass) -> String

Returns the name of a class as a string.

func NSSelectorFromString(String) -> Selector

Returns the selector with a given name.

func NSStringFromSelector(Selector) -> String

Returns a string representation of a given selector.

func NSStringFromProtocol(Protocol) -> String

Returns the name of a protocol as a string.

func NSProtocolFromString(String) -> Protocol?

Returns a the protocol with a given name.

