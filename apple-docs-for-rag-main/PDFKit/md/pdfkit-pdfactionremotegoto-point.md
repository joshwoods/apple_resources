

- PDFKit
- PDFActionRemoteGoTo
-  point 

Instance Property

# point

Sets the point, in page space, on the page referenced by the remote go-to action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var point: CGPoint { get set }
```

**macOS**

``` source
var point: NSPoint { get set }
```

## Parameters 

`point`  

The point on the remote page to go to. If either the x value or the y value of the point is `kPDFDestinationUnspecifiedValue`, no position on the page is specified.

## Discussion

Page space is a 72-dpi coordinate system with the origin at the lower-left corner of the current page.

