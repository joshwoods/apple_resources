

- WebKit
- WebScriptObject
-  setWebScriptValueAt(\_:value:) Deprecated

Instance Method

# setWebScriptValueAt(\_:value:)

Sets the value of a property at the specified index.

macOS 10.4–10.14Deprecated

``` source
func setWebScriptValueAt(
    _ index: UInt32,
    value: Any!
)
```

## Parameters 

`index`  

The index of the property.

`value`  

The value of the property.

## See Also

### Getting and setting properties

func jsObject() -> JSObjectRef!

Returns the JavaScript object corresponding to the receiver.

Deprecated

func removeWebScriptKey(String!)

Removes a property from a scripting environment.

Deprecated

func webScriptValue(at: UInt32) -> Any!

Returns the value of a property at the specified index.

Deprecated

