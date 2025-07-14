

- InputMethodKit
- IMKInputController
-  server() 

Instance Method

# server()

Returns the server object that manages the input controller.

macOS 10.5+

``` source
func server() -> IMKServer!
```

## Return Value

The server object.

## See Also

### Getting the Client and Server Objects

func client() -> (any IMKTextInput &amp; NSObjectProtocol)!

Returns the client object associated with the input controller.

