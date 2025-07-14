

- JavaScriptCore
-  JSValueIsStrictEqual(\_:\_:\_:) 

Function

# JSValueIsStrictEqual(\_:\_:\_:)

Tests whether two JavaScript values are strict equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueIsStrictEqual(
    _ ctx: JSContextRef!,
    _ a: JSValueRef!,
    _ b: JSValueRef!
) -> Bool
```

## Parameters 

`ctx`  

The execution context to use.

`a`  

The first value to test.

`b`  

The second value to test.

## Return Value

true if the two values are strict equal according to the JavaScript `===` operator; otherwise, false.

## See Also

### Comparing Values

func JSValueIsEqual(JSContextRef!, JSValueRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Tests whether two JavaScript values are equal.

func JSValueIsInstanceOfConstructor(JSContextRef!, JSValueRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Tests whether a JavaScript value is an object that the specified constructor creates.

