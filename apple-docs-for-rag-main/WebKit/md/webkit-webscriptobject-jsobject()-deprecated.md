

- WebKit
- WebScriptObject
-  jsObject() Deprecated

Instance Method

# jsObject()

Returns the JavaScript object corresponding to the receiver.

macOS 10.5–10.14Deprecated

``` source
func jsObject() -> JSObjectRef!
```

## Return Value

The JavaScript object corresponding to the receiver in the JavaScriptCore C API.

## See Also

### Getting and setting properties

func removeWebScriptKey(String!)

Removes a property from a scripting environment.

Deprecated

func webScriptValue(at: UInt32) -> Any!

Returns the value of a property at the specified index.

Deprecated

func setWebScriptValueAt(UInt32, value: Any!)

Sets the value of a property at the specified index.

Deprecated

