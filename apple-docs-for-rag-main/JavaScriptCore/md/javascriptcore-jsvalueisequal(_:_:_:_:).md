

- JavaScriptCore
-  JSValueIsEqual(\_:\_:\_:\_:) 

Function

# JSValueIsEqual(\_:\_:\_:\_:)

Tests whether two JavaScript values are equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueIsEqual(
    _ ctx: JSContextRef!,
    _ a: JSValueRef!,
    _ b: JSValueRef!,
    _ exception: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`ctx`  

The execution context to use.

`a`  

The first value to test.

`b`  

The second value to test.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

true if the two values are equal according to the JavaScript `==` operator; false if they’re unequal or the system throws an exception.

## See Also

### Comparing Values

func JSValueIsStrictEqual(JSContextRef!, JSValueRef!, JSValueRef!) -> Bool

Tests whether two JavaScript values are strict equal.

func JSValueIsInstanceOfConstructor(JSContextRef!, JSValueRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Tests whether a JavaScript value is an object that the specified constructor creates.

