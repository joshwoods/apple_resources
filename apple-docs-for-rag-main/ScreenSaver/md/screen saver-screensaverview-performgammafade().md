

- Screen Saver
- ScreenSaverView
-  performGammaFade() 

Type Method

# performGammaFade()

Indicates whether to perform a gradual screen fade when the system starts and stops your screen saver’s animation.

macOS 10.0+

``` source
@MainActor
class func performGammaFade() -> Bool
```

## Discussion

This class method allows the screen saver view to select how the desktop visibly transitions to the screen saver view. When this method returns true, the screen gradually darkens before the animation begins. When it returns false, the screen transitions immediately to the screen saver. The latter behavior is more appropriate if the screen saver animates a screenshot of the desktop, as is the case for optical lens effects. The default is true.

## See Also

### Getting the preferred window behavior

class func backingStoreType() -> NSWindow.BackingStoreType

Returns the type of backing store you want for your screen saver’s window.

