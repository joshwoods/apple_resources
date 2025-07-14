

- AppKit
-  NSShowsServicesMenuItem(\_:) 

Function

# NSShowsServicesMenuItem(\_:)

Specifies whether a Services menu item is currently enabled.

macOS

``` source
func NSShowsServicesMenuItem(_ itemName: String) -> Bool
```

## Discussion

Deprecated. This function simply returns true.

## See Also

### Functions

func NSConvertGlyphsToPackedGlyphs(UnsafeMutablePointer&lt;NSGlyph>, Int, NSMultibyteGlyphPacking, UnsafeMutablePointer&lt;CChar>) -> Int

Prepares a set of glyphs for processing by character-based routines.

Deprecated

static func raiseBadArgumentException(Any!, NSAccessibility.Attribute!, Any!)

Raises an error if the parameter is the wrong type or has an illegal value

Deprecated

func NSReleaseAlertPanel(Any!)

Disposes of an alert panel.

Deprecated

func NSDisableScreenUpdates()

Disables screen updates.

Deprecated

func NSEnableScreenUpdates()

Enables screen updates.

Deprecated

func NSDrawColorTiledRects(NSRect, NSRect, UnsafePointer&lt;NSRectEdge>, AutoreleasingUnsafeMutablePointer&lt;NSColor>, Int) -> NSRect

Draws a single-color, bordered rectangle.

func NSSetShowsServicesMenuItem(String, Bool) -> Int

Specifies whether an item should be included in Services menus.

func NSCopyBits(Int, NSRect, NSPoint)

Copies a bitmap image to the location specified by a destination point.

Deprecated

func NSDottedFrameRect(NSRect)

Draws a bordered rectangle.

func NSReadPixel(NSPoint) -> NSColor?

Reads the color of the pixel at the specified location.

Deprecated

func NSGetWindowServerMemory(Int, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;Int>, AutoreleasingUnsafeMutablePointer&lt;NSString>) -> Int

Returns the amount of memory being used by a context.

Deprecated

static func fileContentsType(forPathExtension: String) -> NSPasteboard.PasteboardType!

Returns a pasteboard type based on the passed file type.

Deprecated

static func fileNameType(forPathExtension: String) -> NSPasteboard.PasteboardType!

Returns a pasteboard type based on the passed file type.

Deprecated

var representedPathExtension: String?

A file type based on the passed pasteboard type.

Deprecated

static func representedPathExtensions(from: [NSPasteboard.PasteboardType]) -> [String]?

Returns an array of file types based on the passed pasteboard types.

Deprecated

