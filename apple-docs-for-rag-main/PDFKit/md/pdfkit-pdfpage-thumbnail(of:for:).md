

- PDFKit
- PDFPage
-  thumbnail(of:for:) 

Instance Method

# thumbnail(of:for:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func thumbnail(
    of size: CGSize,
    for box: PDFDisplayBox
) -> UIImage
```

**macOS**

``` source
func thumbnail(
    of size: NSSize,
    for box: PDFDisplayBox
) -> NSImage
```

## See Also

### Instance Methods

func draw(with: PDFDisplayBox, to: CGContext)

func transform(CGContext, for: PDFDisplayBox)

func transform(for: PDFDisplayBox) -> CGAffineTransform

