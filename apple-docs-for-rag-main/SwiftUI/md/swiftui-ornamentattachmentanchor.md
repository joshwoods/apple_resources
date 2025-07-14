

- SwiftUI
-  OrnamentAttachmentAnchor 

Structure

# OrnamentAttachmentAnchor

An attachment anchor for an ornament.

visionOS 1.0+

``` source
struct OrnamentAttachmentAnchor
```

## Topics

### Getting an anchor

static scene(_:)

The anchor point for the ornament expressed as a unit point relative to the scene.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating an ornament

func ornament&lt;Content>(visibility: Visibility, attachmentAnchor: OrnamentAttachmentAnchor, contentAlignment: Alignment, ornament: () -> Content) -> some View

Presents an ornament.

