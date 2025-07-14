

- PDFKit
- PDFActionRemoteGoTo
-  init(pageIndex:at:fileURL:) 

Initializer

# init(pageIndex:at:fileURL:)

Initializes the remote go-to action with the specified page index, point, and document URL.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
init(
    pageIndex: Int,
    at point: NSPoint,
    fileURL url: URL
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
init(
    pageIndex: Int,
    at point: CGPoint,
    fileURL url: URL
)
```

## Parameters 

`pageIndex`  

The page index of the remote document.

`point`  

The point on the page in the remote document.

`url`  

The URL of the remote PDF document.

## Return Value

An initialized `PDFActionRemoteGoTo` instance, or `NULL` if the object could not be initialized.

## Discussion

The `PDFActionRemoteGoTo` object uses a zero-based page index, not a `PDFPage` object. This simplifies the handling of remote destinations for documents that may not be instantiated yet.

