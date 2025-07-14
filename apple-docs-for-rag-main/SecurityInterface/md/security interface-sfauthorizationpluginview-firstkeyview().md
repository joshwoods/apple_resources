

- Security Interface
- SFAuthorizationPluginView
-  firstKeyView() 

Instance Method

# firstKeyView()

Returns the first view in the keyboard loop of the view.

macOS 10.5+

``` source
func firstKeyView() -> NSView!
```

## Discussion

The default return value of this method is `nil`. When the authorization plug-in calls this method, your subclass should return the first view in the keyboard loop of your custom NSView object.

## See Also

### Setting Up the Keyboard Loop

func firstResponder() -> NSResponder!

Returns the view that should get focus for keyboard events.

func lastKeyView() -> NSView!

Returns the last view in the keyboard loop of the view.

