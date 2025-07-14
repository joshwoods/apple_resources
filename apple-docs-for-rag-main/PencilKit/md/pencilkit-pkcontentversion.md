

- PencilKit
-  PKContentVersion 

Enumeration

# PKContentVersion

Constants that represent versions of PencilKit for backward compatibility.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
enum PKContentVersion
```

## Mentioned in 

Supporting backward compatibility for ink types

## Topics

### Latest version

static var latest: PKContentVersion

A property that returns latest version of PencilKit, which supports all currently available inks.

### Specific versions

case version1

The PencilKit version that supports inks from iPadOS 14 and earlier, including marker, pen, and pencil.

case version2

The PencilKit version that supports inks from iPadOS 17 and earlier, including marker, pen, pencil, monoline, fountain pen, watercolor, and crayon.

case version3

The PencilKit version that supports barrel-roll angle data in inks.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Backward compatibility

Supporting backward compatibility for ink types

Leverage the latest PencilKit features while providing a good user experience in earlier versions of the OS that don’t support those features.

