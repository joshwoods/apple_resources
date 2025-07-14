

- JavaScriptCore
-  JSValueMakeNumber(\_:\_:) 

Function

# JSValueMakeNumber(\_:\_:)

Creates a JavaScript value of the number type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueMakeNumber(
    _ ctx: JSContextRef!,
    _ number: Double
) -> JSValueRef!
```

## Parameters 

`ctx`  

The execution context to use.

`number`  

The double to assign to the newly created JSValueRef.

## Return Value

A JSValueRef of the number type that represents the value of `number`.

## See Also

### Creating Values

func JSValueMakeUndefined(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the undefined type.

func JSValueMakeNull(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the null type.

func JSValueMakeBoolean(JSContextRef!, Bool) -> JSValueRef!

Creates a JavaScript Boolean value.

func JSValueMakeString(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the string type.

func JSValueMakeSymbol(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the symbol type.

