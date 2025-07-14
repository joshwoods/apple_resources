

- AppKit
- NSDocument
-  browseVersions(\_:) 

Instance Method

# browseVersions(\_:)

Opens the Versions browser in the document’s main window.

macOS 10.8+

``` source
@IBAction @MainActor
func browseVersions(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

This is the action of the Browse Saved Versions menu item in a document-based app.

## See Also

### Browsing Document Versions

var isBrowsingVersions: Bool

A Boolean value that indicates whether the document is currently displaying the Versions browser.

func stopBrowsingVersions(completionHandler: (() -> Void)?)

Dismiss the Versions browser for the current document.

