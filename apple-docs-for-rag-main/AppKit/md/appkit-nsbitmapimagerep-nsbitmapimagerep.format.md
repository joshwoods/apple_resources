

- AppKit
- NSBitmapImageRep
-  NSBitmapImageRep.Format 

Structure

# NSBitmapImageRep.Format

Constants that represent bitmap component formats.

macOS

``` source
struct Format
```

## Overview

You can combine these values and pass them to the init(bitmapDataPlanes:pixelsWide:pixelsHigh:bitsPerSample:samplesPerPixel:hasAlpha:isPlanar:colorSpaceName:bitmapFormat:bytesPerRow:bitsPerPixel:) method as the bitmap format. You can access them later in the bitmapFormat property.

## Topics

### Constants

static var alphaFirst: NSBitmapImageRep.Format

A format where the alpha value comes first.

static var alphaNonpremultiplied: NSBitmapImageRep.Format

A format where alpha values are not premultiplied.

static var floatingPointSamples: NSBitmapImageRep.Format

A format where samples are specified using floating-point numbers.

static var sixteenBitBigEndian: NSBitmapImageRep.Format

A 16-bit, big endian format.

static var sixteenBitLittleEndian: NSBitmapImageRep.Format

A 16-bit, little endian format.

static var thirtyTwoBitBigEndian: NSBitmapImageRep.Format

A 32-bit, big endian format.

static var thirtyTwoBitLittleEndian: NSBitmapImageRep.Format

A 32-bit, little endian format.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting Information About Images

var bitmapFormat: NSBitmapImageRep.Format

The format of the bitmap image representation.

var bitsPerPixel: Int

The number of bits allocated for each pixel in each plane of data.

var bytesPerPlane: Int

The number of bytes in each plane or channel of data.

var bytesPerRow: Int

The minimum number of bytes required to specify a scan line in each data plane.

var isPlanar: Bool

A Boolean value that indicates whether the image data is in a planar configuration.

var numberOfPlanes: Int

The number of separate planes into which the image data is organized.

var samplesPerPixel: Int

The number of components for each pixel.

