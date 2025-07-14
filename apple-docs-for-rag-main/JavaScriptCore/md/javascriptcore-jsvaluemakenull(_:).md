

- JavaScriptCore
-  JSValueMakeNull(\_:) 

Function

# JSValueMakeNull(\_:)

Creates a JavaScript value of the null type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueMakeNull(_ ctx: JSContextRef!) -> JSValueRef!
```

## Parameters 

`ctx`  

The execution context to use.

## Return Value

The unique null value.

## See Also

### Creating Values

func JSValueMakeUndefined(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the undefined type.

func JSValueMakeBoolean(JSContextRef!, Bool) -> JSValueRef!

Creates a JavaScript Boolean value.

func JSValueMakeNumber(JSContextRef!, Double) -> JSValueRef!

Creates a JavaScript value of the number type.

func JSValueMakeString(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the string type.

func JSValueMakeSymbol(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the symbol type.

