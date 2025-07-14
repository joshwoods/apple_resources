

- Security Interface
- SFAuthorizationView
-  setDelegate(\_:) 

Instance Method

# setDelegate(\_:)

Sets the delegate for this authorization view.

macOS 10.3+

``` source
@MainActor
func setDelegate(_ delegate: Any!)
```

## Parameters 

`delegate`  

The object to which messages about the state of the authorization object should be sent.

## Discussion

If you want to be notified of state changes (for example, when the user clicks the button), set a delegate and implement the delegate methods described in the delegate methods section.

## See Also

### Setting and getting the delegate for the view

func delegate() -> Any!

Returns the delegate for this view.

