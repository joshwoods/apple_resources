

- AppKit
- NSDocumentController
-  currentDirectory 

Instance Property

# currentDirectory

The directory path to be used as the starting point in the Open panel.

macOS

``` source
@MainActor
var currentDirectory: String? { get }
```

## Discussion

The first valid directory from the following list is returned:

- The directory location where the current document was last saved

- The last directory visited in the Open panel

- The user’s home directory

## See Also

### Managing the Open Dialog

func beginOpenPanel(completionHandler: ([URL]?) -> Void)

Presents an Open dialog and delivers the results to a completion handler as an array of URLs for the chosen files (or `nil`).

func beginOpenPanel(NSOpenPanel, forTypes: [String]?, completionHandler: (Int) -> Void)

Presents a nonmodal Open dialog that displays files you can open from a list of UTIs.

func runModalOpenPanel(NSOpenPanel, forTypes: [String]?) -> Int

Presents a modal Open dialog and limits selection to specific file types.

func urlsFromRunningOpenPanel() -> [URL]?

An array of URLs corresponding to the files selected in a running open panel.

