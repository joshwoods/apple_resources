

- JavaScriptCore
- JSContext
-  setObject(\_:forKeyedSubscript:) 

Instance Method

# setObject(\_:forKeyedSubscript:)

Sets the specified JavaScript property of the context’s global object, allowing subscript setter syntax.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func setObject(
    _ object: Any!,
    forKeyedSubscript key: (any NSCopying & NSObjectProtocol)!
)
```

## Parameters 

`object`  

The value to set for the JavaScript property.

`key`  

The JavaScript property name to use in the context’s global JavaScript object.

## Discussion

This method first constructs a JSValue object from the `key` parameter, then uses that value in JavaScript to set the property in the context’s global object.

Use this method (or Objective-C subscript syntax) to bridge native objects or functions for use in JavaScript. For example, the following code creates a JavaScript function whose implementation is an Objective-C block:

```
```

## See Also

### Accessing JavaScript global state with subscripts

func objectForKeyedSubscript(Any!) -> JSValue!

Returns the value of the specified JavaScript property in the context’s global object, allowing subscript getter syntax.

