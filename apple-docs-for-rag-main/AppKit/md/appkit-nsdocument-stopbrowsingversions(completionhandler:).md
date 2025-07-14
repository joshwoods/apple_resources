

- AppKit
- NSDocument
-  stopBrowsingVersions(completionHandler:) 

Instance Method

# stopBrowsingVersions(completionHandler:)

Dismiss the Versions browser for the current document.

macOS 10.12+

``` source
@MainActor
func stopBrowsingVersions(completionHandler: (() -> Void)? = nil)
```

``` source
@MainActor
func stopBrowsingVersions() async
```

## Parameters 

`completionHandler`  

The completion handler block to call when the Versions browser is fully dismissed. AppKit calls this block on your app’s main thread, waiting for any dismissal animations to complete before calling it. The block block has no return value and no parameters.

## Discussion

## See Also

### Browsing Document Versions

func browseVersions(Any?)

Opens the Versions browser in the document’s main window.

var isBrowsingVersions: Bool

A Boolean value that indicates whether the document is currently displaying the Versions browser.

