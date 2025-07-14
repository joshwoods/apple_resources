

- Core Image
- CIContext
-  CIContextOption 

Structure

# CIContextOption

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
struct CIContextOption
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let allowLowPower: CIContextOption

static let cacheIntermediates: CIContextOption

An option for whether the context caches the contents of any intermediate pixel buffers it uses during rendering.

static let highQualityDownsample: CIContextOption

An option controlling the quality of image downsampling operations performed by the context.

static let memoryTarget: CIContextOption

static let name: CIContextOption

static let outputColorSpace: CIContextOption

A key for the color space to use for images before they are rendered to the context.

static let outputPremultiplied: CIContextOption

An option for whether output rendering by the context produces alpha-premultiplied pixels.

static let priorityRequestLow: CIContextOption

A key for enabling low-priority GPU use.

static let useSoftwareRenderer: CIContextOption

A key for enabling software renderer use. If the associated NSNumber object is `true`, the software renderer is required.

static let workingColorSpace: CIContextOption

A key for the color space to use for image operations.

static let workingFormat: CIContextOption

An option for the color format to use for intermediate results when rendering with the context.

## Relationships

### Conforms To

- Hashable
- RawRepresentable
- Sendable

