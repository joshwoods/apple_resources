

- AppKit
- NSColorPickingDefault
-  alphaControlAddedOrRemoved(\_:) 

Instance Method

# alphaControlAddedOrRemoved(\_:)

Sent when the color panel’s opacity controls have been hidden or displayed.

macOS

``` source
@MainActor
func alphaControlAddedOrRemoved(_ sender: Any?)
```

**Required**

## Parameters 

`sender`  

The color panel sending the message.

## Discussion

This method is invoked automatically when the opacity slider of the `NSColorPanel` is added or removed; you never invoke this method directly.

If the color picker has its own opacity controls, it should hide or display them, depending on whether the sender’s showsAlpha method returns false or true.

## See Also

### Handling Events

func viewSizeChanged(Any?)

Tells the recever when the color panel’s view size changes in a way that might affect the color picker.

**Required**

