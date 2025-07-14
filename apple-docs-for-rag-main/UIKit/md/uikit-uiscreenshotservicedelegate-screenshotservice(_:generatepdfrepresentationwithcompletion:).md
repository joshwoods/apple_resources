

- UIKit
- UIScreenshotServiceDelegate
-  screenshotService(\_:generatePDFRepresentationWithCompletion:) 

Instance Method

# screenshotService(\_:generatePDFRepresentationWithCompletion:)

Generates a high-fidelity PDF version of the entire content in a given window scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+

``` source
@MainActor
optional func screenshotService(
    _ screenshotService: UIScreenshotService,
    generatePDFRepresentationWithCompletion completionHandler: @escaping (Data?, Int, CGRect) -> Void
)
```

``` source
@MainActor
optional func screenshotServiceGeneratePDFRepresentation(_ screenshotService: UIScreenshotService) async -> (Data?, Int, CGRect)
```

## Parameters 

`screenshotService`  

A screenshot service object assigned to the relevant UIWindowScene object. Use the window scene to retrieve the windows of your interface, and generate the PDF content from those windows.

`completionHandler`  

The completion handler block to call with the resulting PDF data. You must call this handler block at the end of your implementation, and pass in the relevant data. This handler block has no return value and takes the following parameters:

PDFData  
The PDF data describing the content in the window scene. If you are unable to produce the PDF data, specify `nil`.

indexOfCurrentPage  
The page index to associate with the PDF data. If your app separates its data into pages of content, use this parameter to specify the current page that the user is viewing. Page indexes are `0`-based, so the first page is at index `0`, the second at index `1`, and so on. Specify `0` if you don’t divide your app’s content into pages.

rectInCurrentPage  
The bounds rectangle in the PDF content that approximates what the user was viewing in your window. Specify this rectangle in the PDF-coordinate space, which has an origin in the bottom-left corner of the content and a y-axis that extends upward.

Specify CGRectZero if you cannot provide the visible rectangle, or if you want the system to always display the PDF content starting at the top of the page.

## Discussion

When the user takes a screenshot of your app, UIKit calls this method to ask you for a PDF version of your content. In your implementation, create a high-fidelity PDF version of your content. At the end of your method, call `completionHandler` with the results.

