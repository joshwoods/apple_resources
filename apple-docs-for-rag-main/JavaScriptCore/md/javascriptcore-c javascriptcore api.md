

- JavaScriptCore
-  C JavaScriptCore API 

API Collection

# C JavaScriptCore API

Browse the alternative C-based APIs for JavaScriptCore.

## Topics

### JavaScriptCore Engine Interface

typealias JSContextGroupRef

A group that associates JavaScript contexts with one another.

typealias JSContextRef

A JavaScript execution context.

typealias JSGlobalContextRef

A global JavaScript execution context.

typealias JSStringRef

A UTF-16 character buffer.

typealias JSClassRef

A JavaScript class.

### JavaScript Data Types

typealias JSValueRef

A JavaScript value.

typealias JSObjectRef

A JavaScript object.

### Script Evaluation

func JSCheckScriptSyntax(JSContextRef!, JSStringRef!, JSStringRef!, Int32, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Checks for syntax errors in a string of JavaScript.

func JSEvaluateScript(JSContextRef!, JSStringRef!, JSObjectRef!, JSStringRef!, Int32, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSValueRef!

Evaluates a string of JavaScript.

func JSGarbageCollect(JSContextRef!)

Performs a JavaScript garbage collection.

### Constants

var JSC_OBJC_API_ENABLED: Int32

