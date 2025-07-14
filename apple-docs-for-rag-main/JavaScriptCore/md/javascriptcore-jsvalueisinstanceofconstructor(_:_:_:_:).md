

- JavaScriptCore
-  JSValueIsInstanceOfConstructor(\_:\_:\_:\_:) 

Function

# JSValueIsInstanceOfConstructor(\_:\_:\_:\_:)

Tests whether a JavaScript value is an object that the specified constructor creates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueIsInstanceOfConstructor(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!,
    _ constructor: JSObjectRef!,
    _ exception: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef to test.

`constructor`  

The constructor to test against.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

true if the value is an object that `constructor` creates, according to the JavaScript `instanceof` operator; otherwise, false.

## See Also

### Comparing Values

func JSValueIsEqual(JSContextRef!, JSValueRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Tests whether two JavaScript values are equal.

func JSValueIsStrictEqual(JSContextRef!, JSValueRef!, JSValueRef!) -> Bool

Tests whether two JavaScript values are strict equal.

