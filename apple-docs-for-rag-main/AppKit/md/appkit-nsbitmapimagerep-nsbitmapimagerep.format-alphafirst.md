

- AppKit
- NSBitmapImageRep
- NSBitmapImageRep.Format
-  alphaFirst 

Type Property

# alphaFirst

A format where the alpha value comes first.

macOS

``` source
static var alphaFirst: NSBitmapImageRep.Format { get }
```

## Discussion

If this option is not specified, alpha values are the last component specified, as in CMYKA and RGBA.

## See Also

### Constants

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

