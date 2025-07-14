

- Image I/O
-  kCGImagePropertyDNGWarpFisheye 

Global Variable

# kCGImagePropertyDNGWarpFisheye

An opcode to unwrap an image captued with a fisheye lens and map it to a perspective projection.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
let kCGImagePropertyDNGWarpFisheye: CFString
```

## See Also

### RAW Data

let kCGImagePropertyDNGOriginalRawFileName: CFString

The file name of the original raw file.

let kCGImagePropertyDNGOriginalRawFileData: CFString

The compressed contents of the original raw file.

let kCGImagePropertyDNGNoiseReductionApplied: CFString

The amount of noise reduction applied to the raw data on a scale of 0.0 to 1.0.

let kCGImagePropertyDNGNewRawImageDigest: CFString

An MD5 digest of the raw image data.

let kCGImagePropertyDNGOriginalRawFileDigest: CFString

An MD5 digest of the data stored for the original raw file data.

let kCGImagePropertyDNGRawImageDigest: CFString

A modified MD5 digest of the raw image data.

let kCGImagePropertyDNGOriginalDefaultFinalSize: CFString

THe default final size of the larger original file that was the source of this proxy.

let kCGImagePropertyDNGOriginalBestQualityFinalSize: CFString

The best-quality final size of the larger original file that was the source of this proxy.

let kCGImagePropertyDNGOriginalDefaultCropSize: CFString

The default crop size of the larger original file that was the source of this proxy.

let kCGImagePropertyDNGRawToPreviewGain: CFString

The gain between the main raw IFD and the preview IFD that contains this tag.

let kCGImagePropertyDNGNoiseProfile: CFString

The amount of noise in the raw image.

let kCGImagePropertyDNGCFALayout: CFString

The spatial layout of the CFA.

let kCGImagePropertyDNGCFAPlaneColor: CFString

A mapping between the values in the CFA pattern tag and the plane numbers in linear raw space.

let kCGImagePropertyDNGOpcodeList1: CFString

The list of opcodes to apply to the raw image, as read directly from the file.

let kCGImagePropertyDNGOpcodeList2: CFString

THe list of opcodes to apply to the raw image, after mapping it to linear reference values.

