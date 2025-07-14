

- WebKit
- WebScriptObject
-  throwException(\_:) Deprecated

Type Method

# throwException(\_:)

Raises an exception in the current script execution context.

macOS 10.4–10.14Deprecated

``` source
class func throwException(_ exceptionMessage: String!) -> Bool
```

## Parameters 

`exceptionMessage`  

The exception message.

## Return Value

true if successful, false otherwise.

## See Also

### Raising exceptions

func setException(String!)

Raises a scripting environment exception in the context of the current object.

Deprecated

