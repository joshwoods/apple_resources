

- AppKit
- NSFontPanel
-  shared 

Type Property

# shared

Returns the single `NSFontPanel` instance for the application, creating it if necessary.

macOS

``` source
@MainActor
class var shared: NSFontPanel { get }
```

## Return Value

The `NSFontPanel` instance for the application.

## See Also

### Related Documentation

Cocoa Text Architecture Guide

class func setFontPanelFactory(AnyClass?)

Sets the class that creates the shared Font panel object.

### Getting the Font Panel

class var sharedFontPanelExists: Bool

Returns true if the shared Font panel has been created, false if it hasn’t.

