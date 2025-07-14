

- JavaScriptCore
-  JSValueMakeSymbol(\_:\_:) 

Function

# JSValueMakeSymbol(\_:\_:)

Creates a JavaScript value of the symbol type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 9.0+visionOS 1.0+

``` source
func JSValueMakeSymbol(
    _ ctx: JSContextRef!,
    _ description: JSStringRef!
) -> JSValueRef!
```

## Parameters 

`ctx`  

The execution context to use.

`description`  

A description of the newly created symbol value.

## Return Value

A unique JSValueRef of the symbol type with a description that matches `description`.

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

func JSValueMakeString(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the string type.

