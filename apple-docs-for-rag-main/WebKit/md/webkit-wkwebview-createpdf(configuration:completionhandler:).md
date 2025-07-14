

- WebKit
- WKWebView
-  createPDF(configuration:completionHandler:) 

Instance Method

# createPDF(configuration:completionHandler:)

Generates PDF data from the web view’s contents asynchronously.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
@MainActor @preconcurrency
func createPDF(
    configuration: WKPDFConfiguration = .init(),
    completionHandler: @escaping @MainActor (Result) -> Void
)
```

## Parameters 

`configuration`  

The object that specifies the portion of the web view to capture as PDF data.

`completionHandler`  

The completion handler to call when the data is ready. This block has no return value and takes the following parameters:

pdfDocumentData  
A data object that contains the PDF data to use for rendering the contents of the web view.

error  
An error object if a problem occurred, or `nil` on success.

## See Also

### Capturing the web view’s content

func takeSnapshot(with: WKSnapshotConfiguration?, completionHandler: (UIImage?, (any Error)?) -> Void)

Generates a platform-native image from the web view’s contents asynchronously.

func pdf(configuration: WKPDFConfiguration) async throws -> Data

Generates PDF data from the web view’s contents asynchronously.

func createWebArchiveData(completionHandler: (Result&lt;Data, any Error>) -> Void)

Creates a web archive of the web view’s current contents asynchronously.

func printOperation(with: NSPrintInfo) -> NSPrintOperation

Returns the print operation object to use when printing the contents of the web view.

class WKSnapshotConfiguration

The configuration data to use when generating an image from a web view’s contents.

class WKPDFConfiguration

The configuration data to use when generating a PDF representation of a web view’s contents.

