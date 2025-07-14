

- Core Graphics
- CGPDFDocument
-  init(\_:) 

Initializer

# init(\_:)

Creates a Core Graphics PDF document using a data provider.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(_ provider: CGDataProvider)
```

## Parameters 

`provider`  

A data provider that supplies the PDF document data.

## Return Value

A new Core Graphics PDF document, or `NULL` if a document can not be created. In Objective-C, you’re responsible for releasing the object using CGPDFDocumentRelease.

## Discussion

Distributing individual pages of a PDF document to separate threads is not supported. If you want to use threads, consider creating a separate document for each thread and operating on a block of pages per thread.

## See Also

### Related Documentation

Quartz 2D Programming Guide

### Creating PDF Documents

init?(CFURL)

Creates a Core Graphics PDF document using data specified by a URL.

