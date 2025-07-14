

- UIKit
- UIPrintInfo
- UIPrintInfo.OutputType
-  UIPrintInfo.OutputType.grayscale 

Case

# UIPrintInfo.OutputType.grayscale

Specifies that the printed content is grayscale. Set the output type to this value when your printable content contains no color—for example, it’s black text only. The default paper is Letter/A4. Output is grayscale quality, duplex. This content type can produce a performance improvement in some cases.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
case grayscale
```

## See Also

### Constants

case general

Specifies that the printed content consists of mixed text, graphics, and images. The default paper is Letter, A4, or similar locale-specific designation. Output is normal quality, duplex.

case photo

Specifies that the printed content consists of black-and-white or color images. The default paper is 4x6, A6, or similar locale-specific designation. Output is high quality, simplex.

case photoGrayscale

Specifies that the printed content is a grayscale image. Set the output type to this value when your printable content contains no color—for example, it’s black text only. The default paper is Letter/A4. Output is high quality grayscale, duplex.

