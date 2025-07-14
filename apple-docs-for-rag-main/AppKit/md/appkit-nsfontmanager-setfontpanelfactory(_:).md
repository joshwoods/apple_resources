

- AppKit
- NSFontManager
-  setFontPanelFactory(\_:) 

Type Method

# setFontPanelFactory(\_:)

Sets the class that creates the shared Font panel object.

macOS

``` source
class func setFontPanelFactory(_ factoryId: AnyClass?)
```

## Parameters 

`factoryId`  

The new font panel factory class, which should be a subclass of `NSFontPanel`.

## Discussion

Call this method before accessing the Font panel in any way, such as in your app delegate’s applicationWillFinishLaunching(_:) method.

## See Also

### Changing the Default Font Conversion Classes

class func setFontManagerFactory(AnyClass?)

Sets the class that creates the shared font manager object.

