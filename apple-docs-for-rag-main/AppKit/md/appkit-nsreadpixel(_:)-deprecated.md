

- AppKit
-  NSReadPixel(\_:) Deprecated

Function

# NSReadPixel(\_:)

Reads the color of the pixel at the specified location.

macOS 10.0–10.14Deprecated

``` source
func NSReadPixel(_ passedPoint: NSPoint) -> NSColor?
```

Deprecated

Use -\[NSBitmapImageRep colorAtX:y:\] to interrogate pixel values. If necessary, use -\[NSView cacheDisplayInRect:toBitmapImageRep:\] to snapshot a view hierarchy into an NSBitmapImageRep.

## Parameters 

`passedPoint`  

The pixel location to read, specified in the current coordinate system.

## Return Value

The color of the pixel at the specified location.

## Discussion

Because the `passedPoint` parameter is relative to the current coordinate system, if you wish to read a pixel from a specific view, you must convert points in the view’s coordinate system to the current coordinate system before calling this function. Alternatively, you can lock focus on the view and then specify the pixel coordinate in the view’s coordinate system.

When mapping the specified point to pixel boundaries, this method rounds to the nearest pixel. For more information on how coordinate points map to the underlying pixels, see Coordinate Systems and Transforms in Cocoa Drawing Guide.

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

