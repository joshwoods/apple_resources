

- PDFKit
-  PDFInterpolationQuality 

Enumeration

# PDFInterpolationQuality

A wrapper for the specified interpolation quality.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.7+tvOS 11.0+visionOS 1.0+

``` source
enum PDFInterpolationQuality
```

## Topics

### Enumeration Cases

case none

The case where no interpolation quality is specified.

case low

The case specifying low interpolation quality.

case high

The case specifying high interpolation quality.

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

### Antialiasing

var shouldAntiAlias: Bool

A Boolean value indicating whether the view is antialiased.

Deprecated

var interpolationQuality: PDFInterpolationQuality

The interpolation quality for images drawn into the `PDFView` context.

