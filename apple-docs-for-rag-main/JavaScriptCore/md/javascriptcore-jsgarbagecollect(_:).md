

- JavaScriptCore
-  JSGarbageCollect(\_:) 

Function

# JSGarbageCollect(\_:)

Performs a JavaScript garbage collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSGarbageCollect(_ ctx: JSContextRef!)
```

## Parameters 

`ctx`  

The execution context to use.

## Discussion

The system doesn’t collect JavaScript values that are on the machine stack, are in a register, are receiving protection from JSValueProtect(_:_:), are the global object of an execution context, or are reachable from any such value.

During JavaScript execution, you don’t have to call this function because the JavaScript engine collects garbage as necessary. The system automatically destroys JavaScript values within a context group when the last reference to the context group releases.

## See Also

### Script Evaluation

func JSCheckScriptSyntax(JSContextRef!, JSStringRef!, JSStringRef!, Int32, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Checks for syntax errors in a string of JavaScript.

func JSEvaluateScript(JSContextRef!, JSStringRef!, JSObjectRef!, JSStringRef!, Int32, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSValueRef!

Evaluates a string of JavaScript.

