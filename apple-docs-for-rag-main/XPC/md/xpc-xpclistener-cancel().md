

- XPC
- XPCListener
-  cancel() 

Instance Method

# cancel()

Cancels a listener.

Mac Catalyst 17.0+macOS 14.0+

``` source
func cancel()
```

## Discussion

Typically you don’t need to explicitly cancel a listener. When the server process exits, the system automatically cancels the listener. In rare circumstances, such as part of a testing infrastructure, you may want to cancel a listener to ensure it doesn’t receive any new messages. Be aware that canceling a listener causes peers attempting to connect to the service to hang.

## See Also

### Managing the life cycle

func activate() throws

Activates an inactive listener.

