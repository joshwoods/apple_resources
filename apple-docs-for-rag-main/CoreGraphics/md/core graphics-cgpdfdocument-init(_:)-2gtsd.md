

- Core Graphics
- CGPDFDocument
-  init(\_:) 

Initializer

# init(\_:)

Creates a Core Graphics PDF document using data specified by a URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(_ url: CFURL)
```

## Parameters 

`url`  

The URL address at which the PDF document data is located.

## Return Value

A new Core Graphics PDF document, or `NULL` if a document could not be created. In Objective-C, you’re responsible for releasing the object using CGPDFDocumentRelease.

## Discussion

Distributing individual pages of a PDF document to separate threads is not supported. If you want to use threads, consider creating a separate document for each thread and operating on a block of pages per thread.

## See Also

### Creating PDF Documents

init?(CGDataProvider)

Creates a Core Graphics PDF document using a data provider.

