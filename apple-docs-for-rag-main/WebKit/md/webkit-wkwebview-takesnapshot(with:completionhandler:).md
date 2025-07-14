

- WebKit
- WKWebView
-  takeSnapshot(with:completionHandler:) 

Instance Method

# takeSnapshot(with:completionHandler:)

Generates a platform-native image from the web view’s contents asynchronously.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

**macOS**

``` source
@MainActor
func takeSnapshot(
    with snapshotConfiguration: WKSnapshotConfiguration?,
    completionHandler: @escaping @MainActor (NSImage?, (any Error)?) -> Void
)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
func takeSnapshot(
    with snapshotConfiguration: WKSnapshotConfiguration?,
    completionHandler: @escaping @MainActor (UIImage?, (any Error)?) -> Void
)
```

**macOS**

``` source
@MainActor
func takeSnapshot(configuration snapshotConfiguration: WKSnapshotConfiguration?) async throws -> NSImage
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
func takeSnapshot(configuration snapshotConfiguration: WKSnapshotConfiguration?) async throws -> UIImage
```

## Parameters 

`snapshotConfiguration`  

The object that specifies the portion of the web view to capture, and other capture-related behaviors.

`completionHandler`  

The completion handler to call when the image is ready. This block has no return value and takes the following parameters:

snapshotImage  
A platform-native image that contains the specified portion of the web view.

error  
An error object if a problem occurred, or `nil` on success.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func takeSnapshot(configuration snapshotConfiguration: WKSnapshotConfiguration?) async throws -> UIImage
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Capturing the web view’s content

func createPDF(configuration: WKPDFConfiguration, completionHandler: (Result&lt;Data, any Error>) -> Void)

Generates PDF data from the web view’s contents asynchronously.

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

