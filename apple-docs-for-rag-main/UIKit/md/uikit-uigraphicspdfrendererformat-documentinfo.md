

- UIKit
- UIGraphicsPDFRendererFormat
-  documentInfo 

Instance Property

# documentInfo

A dictionary that specifies additional information to be associated with the PDFs created by the PDF renderer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var documentInfo: [String : Any] { get set }
```

## Discussion

You can use these keys to specify additional metadata and security information for the PDF, such as the author or the password for accessing it.

The keys used in this dictionary are described in the Auxiliary Dictionary Keys section of the doc://com.apple.documentation/documentation/coregraphics/cgpdfcontext documentation.

