

- UIKit
-  UIGraphicsPDFRendererFormat 

Class

# UIGraphicsPDFRendererFormat

A set of drawing attributes that represents the configuration of a PDF renderer context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsPDFRendererFormat
```

## Overview

Use this subclass of UIGraphicsRendererFormat to provide context configuration parameters to a UIGraphicsPDFRenderer.

Create an instance and then add PDF configuration parameters to the documentInfo dictionary.

The following code demonstrates how you can use a PDF renderer format object to specify the author of the PDFs created by a PDF renderer.

- Swift
- Objective-C

```
let format = UIGraphicsPDFRendererFormat()
format.documentInfo = [ kCGPDFContextAuthor as String : "Kate Bell" ]
let renderer =
  UIGraphicsPDFRenderer(bounds: CGRect(x: 0, y: 0, width: 500, height: 300),
                        format: format)
```

```
UIGraphicsPDFRendererFormat *format = [[UIGraphicsPDFRendererFormat alloc] init];
format.documentInfo = @{ (NSString *)kCGPDFContextAuthor : @"Kate Bell" };
UIGraphicsPDFRenderer *renderer =
    [[UIGraphicsPDFRenderer alloc] initWithBounds:CGRectMake(0, 0, 500, 300)
                                           format:format];
```

## Topics

### Getting the PDF document info

var documentInfo: [String : Any]

A dictionary that specifies additional information to be associated with the PDFs created by the PDF renderer.

## Relationships

### Inherits From

- UIGraphicsRendererFormat

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Graphics contexts

class UIGraphicsRenderer

An abstract base class for creating graphics renderers.

class UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

class UIGraphicsImageRendererContext

The drawing environment for an image renderer.

class UIGraphicsImageRendererFormat

A set of drawing attributes that represents the configuration of an image renderer context.

class UIGraphicsPDFRenderer

A graphics renderer for creating PDFs.

class UIGraphicsPDFRendererContext

The drawing environment for a PDF renderer.

