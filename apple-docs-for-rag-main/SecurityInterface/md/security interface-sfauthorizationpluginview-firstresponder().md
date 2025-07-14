

- Security Interface
- SFAuthorizationPluginView
-  firstResponder() 

Instance Method

# firstResponder()

Returns the view that should get focus for keyboard events.

macOS 10.5+

``` source
func firstResponder() -> NSResponder!
```

## Discussion

The default return value of this method is `nil`. When the authorization plug-in calls this method, your subclass should return the view that should get the focus for keyboard events.

## See Also

### Setting Up the Keyboard Loop

func firstKeyView() -> NSView!

Returns the first view in the keyboard loop of the view.

func lastKeyView() -> NSView!

Returns the last view in the keyboard loop of the view.

