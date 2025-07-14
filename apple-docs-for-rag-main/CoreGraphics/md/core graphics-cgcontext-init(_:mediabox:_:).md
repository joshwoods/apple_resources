

- Core Graphics
- CGContext
-  init(\_:mediaBox:\_:) 

Initializer

# init(\_:mediaBox:\_:)

Creates a URL-based PDF graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    _ url: CFURL,
    mediaBox: UnsafePointer?,
    _ auxiliaryInfo: CFDictionary?
)
```

## Parameters 

`url`  

A Core Foundation URL that specifies where you want to place the resulting PDF file.

`mediaBox`  

A rectangle that specifies the bounds of the PDF. The origin of the rectangle should typically be `(0,0)`. The `CGPDFContextCreateWithURL` function uses this rectangle as the default page media bounding box. If you pass `NULL`, `CGPDFContextCreateWithURL` uses a default page size of 8.5 by 11 inches (612 by 792 points).

`auxiliaryInfo`  

A dictionary that specifies any additional information to be used by the PDF context when generating the PDF file, or `NULL`. The dictionary is retained by the new context, so on return you may safely release it.

## Return Value

A new PDF context, or `NULL` if a context could not be created. In Objective-C, you’re responsible for releasing this object using CGContextRelease.

## Discussion

When you call this function, Core Graphics creates a PDF drawing environment—that is, a graphics context—to your specifications. When you draw into the resulting context, Core Graphics renders your drawing as a series of PDF drawing commands stored in the specified location.

## See Also

### Creating PDF Graphics Contexts

init?(consumer: CGDataConsumer, mediaBox: UnsafePointer&lt;CGRect>?, CFDictionary?)

Creates a PDF graphics context.

Auxiliary Dictionary Keys

Keys for the auxiliary info dictionary you specify when creating a PDF context.

