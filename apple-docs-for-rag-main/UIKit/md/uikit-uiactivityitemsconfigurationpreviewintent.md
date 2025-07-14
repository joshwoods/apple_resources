

- UIKit
-  UIActivityItemsConfigurationPreviewIntent 

Structure

# UIActivityItemsConfigurationPreviewIntent

A structure that specifies the types of activity item previews.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct UIActivityItemsConfigurationPreviewIntent
```

## Topics

### Constants

static let fullSize: UIActivityItemsConfigurationPreviewIntent

A full-size preview image.

static let thumbnail: UIActivityItemsConfigurationPreviewIntent

A thumbnail preview image.

### Initializers

init(String)

Creates a preview intent.

init(rawValue: String)

Creates a preview intent with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing previews

var previewProvider: ((Int, UIActivityItemsConfigurationPreviewIntent, CGSize) -> NSItemProvider?)?

A closure that provides previews for the activity items.

