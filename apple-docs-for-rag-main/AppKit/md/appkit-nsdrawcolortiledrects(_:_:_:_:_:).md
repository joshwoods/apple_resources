

- AppKit
-  NSDrawColorTiledRects(\_:\_:\_:\_:\_:) 

Function

# NSDrawColorTiledRects(\_:\_:\_:\_:\_:)

Draws a single-color, bordered rectangle.

macOS

``` source
func NSDrawColorTiledRects(
    _ boundsRect: NSRect,
    _ clipRect: NSRect,
    _ sides: UnsafePointer,
    _ colors: AutoreleasingUnsafeMutablePointer,
    _ count: Int
) -> NSRect
```

## Parameters 

`boundsRect`  

The bounding rectangle (in the current coordinate system) in which to draw. Since this function is often used to draw the border of a view, this rectangle will typically be that view’s bounds rectangle. Only those parts of `boundsRect` that lie within the `clipRect` are actually drawn.

`clipRect`  

The clipping rectangle to use during drawing.

`sides`  

The sides of the rectangle for which you want to specify custom colors. Each side must have a corresponding entry in the `colors` parameter.

`colors`  

The colors to draw for each of the edges listed in the `sides` parameter.

`count`  

The number of 1.0-unit-wide slices to draw on the specified sides.

## Return Value

The rectangle that lies within the resulting border.

## Discussion

Behaves the same as NSDrawTiledRects(_:_:_:_:_:) except it draws its border using colors from the `colors` array.

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

