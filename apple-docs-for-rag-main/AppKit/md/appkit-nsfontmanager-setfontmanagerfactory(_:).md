

- AppKit
- NSFontManager
-  setFontManagerFactory(\_:) 

Type Method

# setFontManagerFactory(\_:)

Sets the class that creates the shared font manager object.

macOS

``` source
class func setFontManagerFactory(_ factoryId: AnyClass?)
```

## Parameters 

`factoryId`  

The new font manager factory class, which must be a subclass of NSFontManager.

## Discussion

When you call the shared method of NSFontManager, it creates an instance of `aClass`, if no instance already exists. The class in `aClass` must implement `init` as its designated initializer. The default font manager factory is `NSFontManager`.

Call this method before AppKit loads your application’s main nib file, such as in your app delegate’s applicationWillFinishLaunching(_:) method.

## See Also

### Changing the Default Font Conversion Classes

class func setFontPanelFactory(AnyClass?)

Sets the class that creates the shared Font panel object.

