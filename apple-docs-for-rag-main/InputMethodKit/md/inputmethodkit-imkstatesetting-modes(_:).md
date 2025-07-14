

- InputMethodKit
- IMKStateSetting
-  modes(\_:) 

Instance Method

# modes(\_:)

Returns the modes dictionary associated with the input method.

macOS 10.5+

``` source
func modes(_ sender: Any!) -> [AnyHashable : Any]!
```

**Required**

## Parameters 

`sender`  

The client object requesting the modes dictionary.

## Return Value

The modes dictionary associated with the input method.

## Discussion

Typically a client object calls this method to to build the text input menu. By calling the input method rather than reading the modes from the `Info.plist` file, the input method can dynamically modify the modes supported.

