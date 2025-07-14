

- WebKit
- WebScriptObject
-  removeWebScriptKey(\_:) Deprecated

Instance Method

# removeWebScriptKey(\_:)

Removes a property from a scripting environment.

macOS 10.4–10.14Deprecated

``` source
func removeWebScriptKey(_ name: String!)
```

## Parameters 

`name`  

Property to remove.

## See Also

### Getting and setting properties

func jsObject() -> JSObjectRef!

Returns the JavaScript object corresponding to the receiver.

Deprecated

func webScriptValue(at: UInt32) -> Any!

Returns the value of a property at the specified index.

Deprecated

func setWebScriptValueAt(UInt32, value: Any!)

Sets the value of a property at the specified index.

Deprecated

