

- UIKit
- UIPrintInfo
-  UIPrintInfo.OutputType 

Enumeration

# UIPrintInfo.OutputType

Constants that describe the output type, which is an indication of the type of content the app is drawing or providing.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum OutputType
```

## Overview

You use these constants when setting the value of the outputType property of a `UIPrintInfo` object.

## Topics

### Constants

case general

Specifies that the printed content consists of mixed text, graphics, and images. The default paper is Letter, A4, or similar locale-specific designation. Output is normal quality, duplex.

case photo

Specifies that the printed content consists of black-and-white or color images. The default paper is 4x6, A6, or similar locale-specific designation. Output is high quality, simplex.

case grayscale

Specifies that the printed content is grayscale. Set the output type to this value when your printable content contains no color—for example, it’s black text only. The default paper is Letter/A4. Output is grayscale quality, duplex. This content type can produce a performance improvement in some cases.

case photoGrayscale

Specifies that the printed content is a grayscale image. Set the output type to this value when your printable content contains no color—for example, it’s black text only. The default paper is Letter/A4. Output is high quality grayscale, duplex.

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

### Managing print-job attributes

var duplex: UIPrintInfo.Duplex

The duplex mode to use for the print job.

enum Duplex

Constants that describe the duplex mode of a selected printer.

var jobName: String

The name of the print job.

var orientation: UIPrintInfo.Orientation

The orientation of the printed content, portrait or landscape.

enum Orientation

Constants that describe the orientation of printing on a page.

var outputType: UIPrintInfo.OutputType

The kind of printable content.

var printerID: String?

An identifier of the printer to use for the print job.

