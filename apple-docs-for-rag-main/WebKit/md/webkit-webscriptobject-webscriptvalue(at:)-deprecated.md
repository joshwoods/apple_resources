

- WebKit
- WebScriptObject
-  webScriptValue(at:) Deprecated

Instance Method

# webScriptValue(at:)

Returns the value of a property at the specified index.

macOS 10.4–10.14Deprecated

``` source
func webScriptValue(at index: UInt32) -> Any!
```

## Parameters 

`index`  

The index of the property.

## Return Value

The value of a property at `index`. Returns WebUndefined if an exception is thrown in the JavaScript environment.

## Discussion

Accessing property values by index is dependent on the scripting environment.

## See Also

### Getting and setting properties

func jsObject() -> JSObjectRef!

Returns the JavaScript object corresponding to the receiver.

Deprecated

func removeWebScriptKey(String!)

Removes a property from a scripting environment.

Deprecated

func setWebScriptValueAt(UInt32, value: Any!)

Sets the value of a property at the specified index.

Deprecated

