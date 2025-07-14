

- JavaScriptCore
-  JSEvaluateScript(\_:\_:\_:\_:\_:\_:) 

Function

# JSEvaluateScript(\_:\_:\_:\_:\_:\_:)

Evaluates a string of JavaScript.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSEvaluateScript(
    _ ctx: JSContextRef!,
    _ script: JSStringRef!,
    _ thisObject: JSObjectRef!,
    _ sourceURL: JSStringRef!,
    _ startingLineNumber: Int32,
    _ exception: UnsafeMutablePointer!
) -> JSValueRef!
```

## Parameters 

`ctx`  

The execution context to use.

`script`  

A JSStringRef that contains the script to evaluate.

`thisObject`  

The object to use as `this` or `NULL` to use the global object as `this`.

`sourceURL`  

A JSStringRef that contains a URL for the script’s source file. The system only uses this when reporting exceptions. Pass `NULL` to omit source file information in exceptions.

`startingLineNumber`  

An integer value that specifies the script’s starting line number in the file at `sourceURL`. The system only uses this when reporting exceptions.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

The value that results from evaluating `script`, or `NULL` if the system throws an exception.

## See Also

### Script Evaluation

func JSCheckScriptSyntax(JSContextRef!, JSStringRef!, JSStringRef!, Int32, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Checks for syntax errors in a string of JavaScript.

func JSGarbageCollect(JSContextRef!)

Performs a JavaScript garbage collection.

