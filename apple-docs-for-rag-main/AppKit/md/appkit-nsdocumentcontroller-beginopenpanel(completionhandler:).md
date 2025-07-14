

- AppKit
- NSDocumentController
-  beginOpenPanel(completionHandler:) 

Instance Method

# beginOpenPanel(completionHandler:)

Presents an Open dialog and delivers the results to a completion handler as an array of URLs for the chosen files (or `nil`).

macOS 10.8+

``` source
@MainActor
func beginOpenPanel(completionHandler: @escaping ([URL]?) -> Void)
```

``` source
@MainActor
func beginOpenPanel() async -> [URL]?
```

## Parameters 

`completionHandler`  

The completion handler that is called when the user clicks the OK or Cancel button in the open panel.

## Discussion

This method presents either a modal or nonmodal open panel, depending on which methods are overridden. Although you can call this method in other circumstances, this method is most commonly called by openDocument(_:) in response to the user choosing Open… from the File menu.

If you override openDocument(_:), you should typically call this method instead of calling beginOpenPanel(_:forTypes:completionHandler:) or urlsFromRunningOpenPanel() directly, because this method runs the modal panel in a way that is backwards compatible with subclasses that override runModalOpenPanel(_:forTypes:) without overriding beginOpenPanel(_:forTypes:completionHandler:). Also, its completion handler determines which button the user pressed (to determine whether to return the array or `nil`) and orders out the open panel.

You can override this method to change the open panel presentation (adding an accessory view, for example) or change the UTI array that limits which files are selectable.

The default implementation of this method calls either urlsFromRunningOpenPanel() to run a modal open panel or beginOpenPanel(_:forTypes:completionHandler:) to begin a nonmodal open panel. If the user chooses to open files, the default implementation calls the completion handler with a `nil` array parameter. If the user cancels the Open dialog, the default implementation calls the completion handler with a `nil` array parameter.

If you override this method, your method should typically call the underlying method on `super` because of the additional code that it provides for free. Specifically, this method runs the modal panel in a way that is backwards compatible with subclasses that override runModalOpenPanel(_:forTypes:) without overriding beginOpenPanel(_:forTypes:completionHandler:). Also, its completion handler determines which button the user pressed (to determine whether to return the array or `nil`) and orders out the open panel.

## See Also

### Managing the Open Dialog

func beginOpenPanel(NSOpenPanel, forTypes: [String]?, completionHandler: (Int) -> Void)

Presents a nonmodal Open dialog that displays files you can open from a list of UTIs.

func runModalOpenPanel(NSOpenPanel, forTypes: [String]?) -> Int

Presents a modal Open dialog and limits selection to specific file types.

var currentDirectory: String?

The directory path to be used as the starting point in the Open panel.

func urlsFromRunningOpenPanel() -> [URL]?

An array of URLs corresponding to the files selected in a running open panel.

