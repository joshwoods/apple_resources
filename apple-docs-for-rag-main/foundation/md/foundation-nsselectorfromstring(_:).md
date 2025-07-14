

- Foundation
-  NSSelectorFromString(\_:) 

Function

# NSSelectorFromString(\_:)

Returns the selector with a given name.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSSelectorFromString(_ aSelectorName: String) -> Selector
```

## Parameters 

`aSelectorName`  

A string of any length, with any characters, that represents the name of a selector.

## Return Value

The selector named by `aSelectorName`. If `aSelectorName` is `nil`, or cannot be converted to UTF-8 (this should be only due to insufficient memory), returns `(SEL)0`.

## Discussion

To make a selector, NSSelectorFromString(_:) passes a UTF-8 encoded character representation of `aSelectorName` to doc://com.apple.documentation/documentation/objectivec/1418557-sel_registername and returns the value returned by that function. Note, therefore, that if the selector does not exist it is registered and the newly-registered selector is returned.

Recall that a colon (”:”) is part of a method name; `setHeight` is not the same as `setHeight:`.

## See Also

### Type Lookup

func NSClassFromString(String) -> AnyClass?

Obtains a class by name.

func NSStringFromClass(AnyClass) -> String

Returns the name of a class as a string.

func NSStringFromSelector(Selector) -> String

Returns a string representation of a given selector.

func NSStringFromProtocol(Protocol) -> String

Returns the name of a protocol as a string.

func NSProtocolFromString(String) -> Protocol?

Returns a the protocol with a given name.

