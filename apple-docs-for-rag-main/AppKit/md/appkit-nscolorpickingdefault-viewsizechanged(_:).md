

- AppKit
- NSColorPickingDefault
-  viewSizeChanged(\_:) 

Instance Method

# viewSizeChanged(\_:)

Tells the recever when the color panel’s view size changes in a way that might affect the color picker.

macOS

``` source
@MainActor
func viewSizeChanged(_ sender: Any?)
```

**Required**

## Parameters 

`sender`  

The `NSColorPanel` that contains the color picker.

## Discussion

Use this method to perform special preparation when resizing the color picker’s view. Because this method is invoked only as appropriate, it’s better to implement this method than to override the method `superviewSizeChanged:` for the `NSView` in which the color picker’s user interface is contained.

## See Also

### Related Documentation

func provideNewView(Bool) -> NSView

Returns the view containing the receiver’s user interface.

**Required**

### Handling Events

func alphaControlAddedOrRemoved(Any?)

Sent when the color panel’s opacity controls have been hidden or displayed.

**Required**

