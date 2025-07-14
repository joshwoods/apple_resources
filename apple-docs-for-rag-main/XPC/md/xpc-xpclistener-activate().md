

- XPC
- XPCListener
-  activate() 

Instance Method

# activate()

Activates an inactive listener.

Mac Catalyst 17.0+macOS 14.0+

``` source
func activate() throws
```

## Discussion

If you create an inactive listener using the inactive flag, be sure to activate it before releasing the last reference to the listener. Releasing the last reference to an inactive listener crashes.

If activation fails, the system automatically cancels the listener.

## See Also

### Managing the life cycle

func cancel()

Cancels a listener.

