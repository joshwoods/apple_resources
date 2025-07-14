

- WebKit
- WKWebView
-  printOperation(with:) 

Instance Method

# printOperation(with:)

Returns the print operation object to use when printing the contents of the web view.

macOS 11.0+

``` source
@MainActor
func printOperation(with printInfo: NSPrintInfo) -> NSPrintOperation
```

## Parameters 

`printInfo`  

The printer information object to use when configuring the print operation.

## Return Value

The print operation object to use when printing the web view, or `nil` if printing is not supported.

## See Also

### Capturing the web view’s content

func takeSnapshot(with: WKSnapshotConfiguration?, completionHandler: (UIImage?, (any Error)?) -> Void)

Generates a platform-native image from the web view’s contents asynchronously.

func createPDF(configuration: WKPDFConfiguration, completionHandler: (Result&lt;Data, any Error>) -> Void)

Generates PDF data from the web view’s contents asynchronously.

func pdf(configuration: WKPDFConfiguration) async throws -> Data

Generates PDF data from the web view’s contents asynchronously.

func createWebArchiveData(completionHandler: (Result&lt;Data, any Error>) -> Void)

Creates a web archive of the web view’s current contents asynchronously.

class WKSnapshotConfiguration

The configuration data to use when generating an image from a web view’s contents.

class WKPDFConfiguration

The configuration data to use when generating a PDF representation of a web view’s contents.

