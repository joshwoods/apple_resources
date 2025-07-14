

- JavaScriptCore
- JSContext
-  objectForKeyedSubscript(\_:) 

Instance Method

# objectForKeyedSubscript(\_:)

Returns the value of the specified JavaScript property in the context’s global object, allowing subscript getter syntax.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func objectForKeyedSubscript(_ key: Any!) -> JSValue!
```

## Parameters 

`key`  

The name of a JavaScript property in the context’s global JavaScript object.

## Return Value

The JavaScript property named by `key`, or `nil` if no such field or function exists.

## Discussion

This method first constructs a JSValue object from the `key` parameter, then uses that value in JavaScript to look up the name of a property in the context’s global object.

## See Also

### Accessing JavaScript global state with subscripts

func setObject(Any!, forKeyedSubscript: (any NSCopying &amp; NSObjectProtocol)!)

Sets the specified JavaScript property of the context’s global object, allowing subscript setter syntax.

