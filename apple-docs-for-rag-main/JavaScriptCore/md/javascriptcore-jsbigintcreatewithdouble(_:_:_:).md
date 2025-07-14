

- JavaScriptCore
-  JSBigIntCreateWithDouble(\_:\_:\_:) 

Function

# JSBigIntCreateWithDouble(\_:\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 9.0+visionOS 2.0+

``` source
func JSBigIntCreateWithDouble(
    _ ctx: JSContextRef,
    _ value: Double,
    _ exception: UnsafeMutablePointer?
) -> JSValueRef
```

## Discussion

```
@function
@abstract         Creates a JavaScript BigInt with a double.
@param ctx        The execution context to use.
@param value      The value to copy into the new BigInt JSValue.
@param exception  A pointer to a JSValueRef in which to store an exception, if any. To reliable detect exception, initialize this to null before the call. Pass NULL if you do not care to store an exception.
@result           A BigInt JSValue of the value, or NULL if an exception is thrown.
@discussion       If the value is not an integer, an exception is thrown.
```

