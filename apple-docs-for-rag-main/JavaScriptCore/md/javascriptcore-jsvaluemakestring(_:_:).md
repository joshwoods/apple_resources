

- JavaScriptCore
-  JSValueMakeString(\_:\_:) 

Function

# JSValueMakeString(\_:\_:)

Creates a JavaScript value of the string type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueMakeString(
    _ ctx: JSContextRef!,
    _ string: JSStringRef!
) -> JSValueRef!
```

## Parameters 

`ctx`  

The execution context to use.

`string`  

The JSStringRef to assign to the newly created JSValueRef. The newly created JSValueRef retains `string`, and releases it upon garbage collection.

## Return Value

A JSValueRef of the string type that represents the value of `string`.

## See Also

### Creating Values

func JSValueMakeUndefined(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the undefined type.

func JSValueMakeNull(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the null type.

func JSValueMakeBoolean(JSContextRef!, Bool) -> JSValueRef!

Creates a JavaScript Boolean value.

func JSValueMakeNumber(JSContextRef!, Double) -> JSValueRef!

Creates a JavaScript value of the number type.

func JSValueMakeSymbol(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the symbol type.

