

- AppKit
- NSFontManager
-  shared 

Type Property

# shared

Returns the shared instance of the font manager for the application, creating it if necessary.

macOS

``` source
class var shared: NSFontManager { get }
```

## Return Value

The shared font manager.

## See Also

### Related Documentation

Cocoa Text Architecture Guide

class func setFontManagerFactory(AnyClass?)

Sets the class that creates the shared font manager object.

