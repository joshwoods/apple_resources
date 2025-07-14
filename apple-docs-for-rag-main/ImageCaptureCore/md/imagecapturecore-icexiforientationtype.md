

- ImageCaptureCore
-  ICEXIFOrientationType 

Enumeration

# ICEXIFOrientationType

The file’s orientation type.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum ICEXIFOrientationType
```

## Overview

The meaning of this value is defined by the `EXIF` specification. Here is what the letter *F* would look like if it were tagged correctly and displayed by a program that ignores the orientation tag (thus showing the stored image):

```
               1             2             3             4

            8888888       8888888            88       88
            88                 88            88       88
            8888             8888          8888       8888
            88                 88            88       88
            88                 88       8888888       8888888

               5             6             7             8

            8888888888    88                    88    8888888888
            88  88        88  88            88  88        88  88
            88            8888888888    8888888888            88
```

## Topics

### Constants

case orientation1

Normal

case orientation2

Flipped horizontally

case orientation3

Rotated 180°

case orientation4

Flipped vertically

case orientation5

Rotated 90° CCW and flipped vertically

case orientation6

Rotated 90° CCW

case orientation7

Rotated 90° CW and flipped vertically

case orientation8

Rotated 90° CW

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a File’s EXIF Data

var orientation: ICEXIFOrientationType

The orientation to use when downloading the image.

var exifCreationDate: Date?

The `EXIF` creation date of the file.

var exifModificationDate: Date?

The `EXIF` modification date of the file.

