

- Screen Saver
- ScreenSaverView
-  backingStoreType() 

Type Method

# backingStoreType()

Returns the type of backing store you want for your screen saver’s window.

macOS 10.0+

``` source
@MainActor
class func backingStoreType() -> NSWindow.BackingStoreType
```

## Discussion

This method returns NSWindow.BackingStoreType.buffered by default. If you want to change the backing store type, override this method and return a new value. If you override the method, you don’t need to call the inherited version.

## See Also

### Getting the preferred window behavior

class func performGammaFade() -> Bool

Indicates whether to perform a gradual screen fade when the system starts and stops your screen saver’s animation.

