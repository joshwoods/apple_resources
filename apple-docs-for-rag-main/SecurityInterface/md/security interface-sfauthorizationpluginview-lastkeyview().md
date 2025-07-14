

- Security Interface
- SFAuthorizationPluginView
-  lastKeyView() 

Instance Method

# lastKeyView()

Returns the last view in the keyboard loop of the view.

macOS 10.5+

``` source
func lastKeyView() -> NSView!
```

## Discussion

The default return value of this method is `nil`. When the authorization plug-in calls this method, your subclass should return the last view in the keyboard loop of your custom NSView object.

## See Also

### Setting Up the Keyboard Loop

func firstKeyView() -> NSView!

Returns the first view in the keyboard loop of the view.

func firstResponder() -> NSResponder!

Returns the view that should get focus for keyboard events.

