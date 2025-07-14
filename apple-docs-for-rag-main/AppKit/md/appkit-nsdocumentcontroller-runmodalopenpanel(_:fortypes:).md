

- AppKit
- NSDocumentController
-  runModalOpenPanel(\_:forTypes:) 

Instance Method

# runModalOpenPanel(\_:forTypes:)

Presents a modal Open dialog and limits selection to specific file types.

macOS

``` source
@MainActor
func runModalOpenPanel(
    _ openPanel: NSOpenPanel,
    forTypes types: [String]?
) -> Int
```

## Parameters 

`openPanel`  

The open panel to display.

`types`  

An array of allowable types to open.

## Discussion

This method is called by the urlsFromRunningOpenPanel() method. It calls the `NSOpenPanel` runModalForTypes: method, passing the `openPanel` object and the file extensions associated with a document type. The `extensions` parameter may also contain encoded HFS file types as well as filename extensions.

## See Also

### Managing the Open Dialog

func beginOpenPanel(completionHandler: ([URL]?) -> Void)

Presents an Open dialog and delivers the results to a completion handler as an array of URLs for the chosen files (or `nil`).

func beginOpenPanel(NSOpenPanel, forTypes: [String]?, completionHandler: (Int) -> Void)

Presents a nonmodal Open dialog that displays files you can open from a list of UTIs.

var currentDirectory: String?

The directory path to be used as the starting point in the Open panel.

func urlsFromRunningOpenPanel() -> [URL]?

An array of URLs corresponding to the files selected in a running open panel.

