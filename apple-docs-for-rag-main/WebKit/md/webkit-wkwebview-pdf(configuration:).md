

- WebKit
- WKWebView
-  pdf(configuration:) 

Instance Method

# pdf(configuration:)

Generates PDF data from the web view’s contents asynchronously.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOS

``` source
@MainActor @preconcurrency
func pdf(configuration: WKPDFConfiguration = .init()) async throws -> Data
```

## Parameters 

`configuration`  

The object that specifies the portion of the web view to capture as PDF data.

## Return Value

A data object that contains the PDF data to use for rendering the contents of the web view.

## See Also

### Capturing the web view’s content

func takeSnapshot(with: WKSnapshotConfiguration?, completionHandler: (UIImage?, (any Error)?) -> Void)

Generates a platform-native image from the web view’s contents asynchronously.

func createPDF(configuration: WKPDFConfiguration, completionHandler: (Result&lt;Data, any Error>) -> Void)

Generates PDF data from the web view’s contents asynchronously.

func createWebArchiveData(completionHandler: (Result&lt;Data, any Error>) -> Void)

Creates a web archive of the web view’s current contents asynchronously.

func printOperation(with: NSPrintInfo) -> NSPrintOperation

Returns the print operation object to use when printing the contents of the web view.

class WKSnapshotConfiguration

The configuration data to use when generating an image from a web view’s contents.

class WKPDFConfiguration

The configuration data to use when generating a PDF representation of a web view’s contents.

