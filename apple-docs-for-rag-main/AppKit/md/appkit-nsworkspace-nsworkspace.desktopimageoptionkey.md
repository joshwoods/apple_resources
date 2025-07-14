

- AppKit
- NSWorkspace
-  NSWorkspace.DesktopImageOptionKey 

Structure

# NSWorkspace.DesktopImageOptionKey

Keys that indicate how to display a new desktop image.

macOS

``` source
struct DesktopImageOptionKey
```

## Discussion

Specify the following keys when calling the setDesktopImageURL(_:for:options:) method.

## Topics

### Option Keys

static let imageScaling: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when scaling the image.

static let allowClipping: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when clipping the image.

static let fillColor: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when filling the empty space around the image.

### Initializers

init(rawValue: String)

Initializes an option key using the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the Desktop Image

func desktopImageURL(for: NSScreen) -> URL?

Returns the URL for the desktop image for the given screen.

func setDesktopImageURL(URL, for: NSScreen, options: [NSWorkspace.DesktopImageOptionKey : Any]) throws

Sets the desktop image for the given screen to the image at the specified URL.

func desktopImageOptions(for: NSScreen) -> [NSWorkspace.DesktopImageOptionKey : Any]?

Returns the desktop image options for the given screen.

