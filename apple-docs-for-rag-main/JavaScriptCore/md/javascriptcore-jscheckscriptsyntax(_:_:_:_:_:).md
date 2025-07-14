

- JavaScriptCore
-  JSCheckScriptSyntax(\_:\_:\_:\_:\_:) 

Function

# JSCheckScriptSyntax(\_:\_:\_:\_:\_:)

Checks for syntax errors in a string of JavaScript.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSCheckScriptSyntax(
    _ ctx: JSContextRef!,
    _ script: JSStringRef!,
    _ sourceURL: JSStringRef!,
    _ startingLineNumber: Int32,
    _ exception: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`ctx`  

The execution context to use.

`script`  

A JSStringRef that contains the script to check for syntax errors.

`sourceURL`  

A JSStringRef that contains a URL for the script’s source file. The system only uses this when reporting exceptions. Pass `NULL` to omit source file information in exceptions.

`startingLineNumber`  

An integer value that specifies the script’s starting line number in the file at `sourceURL`. The system only uses this when reporting exceptions.

`exception`  

A pointer to a JSValueRef to store a syntax error exception in, if any. Pass `NULL` to ignore any syntax error exception.

## Return Value

true if the script is syntactically correct; otherwise, false.

## See Also

### Script Evaluation

func JSEvaluateScript(JSContextRef!, JSStringRef!, JSObjectRef!, JSStringRef!, Int32, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSValueRef!

Evaluates a string of JavaScript.

func JSGarbageCollect(JSContextRef!)

Performs a JavaScript garbage collection.

