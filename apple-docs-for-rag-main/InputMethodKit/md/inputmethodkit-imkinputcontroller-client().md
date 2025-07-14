

- InputMethodKit
- IMKInputController
-  client() 

Instance Method

# client()

Returns the client object associated with the input controller.

macOS 10.5+

``` source
func client() -> (any IMKTextInput & NSObjectProtocol)!
```

## Return Value

The client object.

## Discussion

The client object conforms to the `IMKTextInput` protocol.

## See Also

### Getting the Client and Server Objects

func server() -> IMKServer!

Returns the server object that manages the input controller.

