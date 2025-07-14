

- AppKit
-  NSGetWindowServerMemory(\_:\_:\_:\_:) Deprecated

Function

# NSGetWindowServerMemory(\_:\_:\_:\_:)

Returns the amount of memory being used by a context.

macOS 10.0–10.14Deprecated

``` source
func NSGetWindowServerMemory(
    _ context: Int,
    _ virtualMemory: UnsafeMutablePointer,
    _ windowBackingMemory: UnsafeMutablePointer,
    _ windowDumpString: AutoreleasingUnsafeMutablePointer
) -> Int
```

Deprecated

Doesn't return anything useful since 10.0

## Discussion

Calculates the amount of memory being used at the moment by the given `context`. If `NULL` is passed for `context`, the current context is used. The amount of virtual memory used by the current context is returned in the int pointed to by `virtualMemory`; the amount of window backing store used by windows owned by the current context is returned in the int pointed to by `windowBackingMemory`. The sum of these two numbers is the amount of the memory that this context is responsible for.

Calculating these numbers takes some time to execute; thus, calling this function in normal operation is not recommended.

If `nil` is not passed in for `windowDumpStream`, the information returned is echoed to the specified stream. This fact can be useful for finding out more about which windows are using up your storage.

Normally, `NSGetWindowServerMemory` returns 0. If `NULL` is passed for `context` and there’s no current display context, this function returns –1.

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

func NSShowsServicesMenuItem(String) -> Bool

Specifies whether a Services menu item is currently enabled.

func NSDottedFrameRect(NSRect)

Draws a bordered rectangle.

func NSReadPixel(NSPoint) -> NSColor?

Reads the color of the pixel at the specified location.

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

