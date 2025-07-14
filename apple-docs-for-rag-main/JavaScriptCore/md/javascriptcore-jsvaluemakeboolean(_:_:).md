

- JavaScriptCore
-  JSValueMakeBoolean(\_:\_:) 

Function

# JSValueMakeBoolean(\_:\_:)

Creates a JavaScript Boolean value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueMakeBoolean(
    _ ctx: JSContextRef!,
    _ boolean: Bool
) -> JSValueRef!
```

## Parameters 

`ctx`  

The execution context to use.

`boolean`  

The Boolean value to assign to the newly created JSValueRef.

## Return Value

A JSValueRef of the Boolean type that represents the value of `boolean`.

## See Also

### Creating Values

func JSValueMakeUndefined(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the undefined type.

func JSValueMakeNull(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the null type.

func JSValueMakeNumber(JSContextRef!, Double) -> JSValueRef!

Creates a JavaScript value of the number type.

func JSValueMakeString(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the string type.

func JSValueMakeSymbol(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the symbol type.

