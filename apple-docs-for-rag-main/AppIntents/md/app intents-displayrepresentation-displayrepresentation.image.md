

- App Intents
- DisplayRepresentation
-  DisplayRepresentation.Image 

Structure

# DisplayRepresentation.Image

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Image
```

## Topics

### Structures

struct DisplayStyle

The style with which to display the image for this `DisplayRepresentation`.

### Operators

static func == (DisplayRepresentation.Image, DisplayRepresentation.Image) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(data: Data, isTemplate: Bool?)

Creates an image object from the specified data.

init(data: Data, isTemplate: Bool?, displayStyle: DisplayRepresentation.Image.DisplayStyle)

Creates an image from the specified data, specifying the display style.

init(named: String, isTemplate: Bool?)

Creates an image object from an image file in the extension’s bundle.

init(named: String, isTemplate: Bool?, displayStyle: DisplayRepresentation.Image.DisplayStyle)

Creates an image from an image file in the extension’s bundle, specifying the display style.

init(systemName: String, isTemplate: Bool?)

Creates an image object that contains the specified system symbol image.

init?(systemName: String, tintColor: UIColor?, symbolConfiguration: UIImage.SymbolConfiguration?)

Creates an image object backed by the given SF Symbol name, with optional configuration options.

init?(systemName: String, tintColor: NSColor?, symbolConfiguration: NSImage.SymbolConfiguration?)

Creates an image object backed by the given SF Symbol name, with optional configuration options.

init(url: URL, isTemplate: Bool?)

Creates an image object from an image file in the local file system.

init(url: URL, isTemplate: Bool?, displayStyle: DisplayRepresentation.Image.DisplayStyle)

Creates an image from an image file in the local file system, specifying the display style.

init(url: URL, width: Double, height: Double, isTemplate: Bool?)

Creates an image object, of the specified size, from an image file in the local file system.

init(url: URL, width: Double, height: Double, isTemplate: Bool?, displayStyle: DisplayRepresentation.Image.DisplayStyle)

Creates an image, of the specified size, from an image file in the local file system, specifying the display style.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Displaying the content

var title: LocalizedStringResource

var subtitle: LocalizedStringResource?

var image: DisplayRepresentation.Image?

