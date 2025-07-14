

- UIKit
- UIGraphicsPDFRendererContext
-  beginPage(withBounds:pageInfo:) 

Instance Method

# beginPage(withBounds:pageInfo:)

Marks the beginning of a new page in the PDF context and configures it using the specified values.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func beginPage(
    withBounds bounds: CGRect,
    pageInfo: [String : Any]
)
```

## Parameters 

`bounds`  

A rectangle that specifies the size and location of the new PDF page. This rectangle corresponds to the media box in PDF terminology.

`pageInfo`  

A dictionary that specifies additional page-related information, such as the boxes that define different parts of the page. For a list of keys you can include in this dictionary, see `Box Dictionary Keys` in doc://com.apple.documentation/documentation/coregraphics/cgpdfcontext.

## Discussion

This function ends any previous page before beginning a new one. It sets the media box of the new page to the value in the kCGPDFContextMediaBox key of the `pageInfo` dictionary, or to the value in the bounds parameter if the dictionary does not contain the key.

## See Also

### Marking new pages

func beginPage()

Marks the beginning of a new page in the PDF context and configures it using default values.

