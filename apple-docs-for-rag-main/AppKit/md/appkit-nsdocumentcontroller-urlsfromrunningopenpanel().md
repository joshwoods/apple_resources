

- AppKit
- NSDocumentController
-  urlsFromRunningOpenPanel() 

Instance Method

# urlsFromRunningOpenPanel()

An array of URLs corresponding to the files selected in a running open panel.

macOS

``` source
@MainActor
func urlsFromRunningOpenPanel() -> [URL]?
```

## Discussion

Accessing this property creates an NSOpenPanel object and runs it using the runModalOpenPanel(_:forTypes:) method. When the user dismisses the panel, the returned value is an array of URLs corresponding to the files chosen by the user. The value is `nil` if the user cancels the Open panel or makes no selection.

## See Also

### Managing the Open Dialog

func beginOpenPanel(completionHandler: ([URL]?) -> Void)

Presents an Open dialog and delivers the results to a completion handler as an array of URLs for the chosen files (or `nil`).

func beginOpenPanel(NSOpenPanel, forTypes: [String]?, completionHandler: (Int) -> Void)

Presents a nonmodal Open dialog that displays files you can open from a list of UTIs.

func runModalOpenPanel(NSOpenPanel, forTypes: [String]?) -> Int

Presents a modal Open dialog and limits selection to specific file types.

var currentDirectory: String?

The directory path to be used as the starting point in the Open panel.

