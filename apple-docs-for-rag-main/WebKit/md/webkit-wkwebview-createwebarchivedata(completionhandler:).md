

- WebKit
- WKWebView
-  createWebArchiveData(completionHandler:) 

Instance Method

# createWebArchiveData(completionHandler:)

Creates a web archive of the web view’s current contents asynchronously.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
@MainActor @preconcurrency
func createWebArchiveData(completionHandler: @escaping @MainActor (Result) -> Void)
```

## Parameters 

`completionHandler`  

The completion handler block to call when the web archive data is ready. This block has no return value and takes the following parameters:

data  
A data object that contains the web archive.

error  
An error object if an error occurs, or `nil` on success.

## See Also

### Capturing the web view’s content

func takeSnapshot(with: WKSnapshotConfiguration?, completionHandler: (UIImage?, (any Error)?) -> Void)

Generates a platform-native image from the web view’s contents asynchronously.

func createPDF(configuration: WKPDFConfiguration, completionHandler: (Result&lt;Data, any Error>) -> Void)

Generates PDF data from the web view’s contents asynchronously.

func pdf(configuration: WKPDFConfiguration) async throws -> Data

Generates PDF data from the web view’s contents asynchronously.

func printOperation(with: NSPrintInfo) -> NSPrintOperation

Returns the print operation object to use when printing the contents of the web view.

class WKSnapshotConfiguration

The configuration data to use when generating an image from a web view’s contents.

class WKPDFConfiguration

The configuration data to use when generating a PDF representation of a web view’s contents.

