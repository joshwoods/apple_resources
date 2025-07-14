

- AppKit
- NSDocument
-  isBrowsingVersions 

Instance Property

# isBrowsingVersions

A Boolean value that indicates whether the document is currently displaying the Versions browser.

macOS 10.12+

``` source
@MainActor
var isBrowsingVersions: Bool { get }
```

## Discussion

The value of this property is true when the versions browser is visible.

## See Also

### Browsing Document Versions

func browseVersions(Any?)

Opens the Versions browser in the document’s main window.

func stopBrowsingVersions(completionHandler: (() -> Void)?)

Dismiss the Versions browser for the current document.

