

- AppKit
- NSWorkspace
-  activateFileViewerSelecting(\_:) 

Instance Method

# activateFileViewerSelecting(\_:)

Activates the Finder, and opens one or more windows selecting the specified files.

macOS 10.6+

``` source
func activateFileViewerSelecting(_ fileURLs: [URL])
```

## Parameters 

`fileURLs`  

The files to select and display in the Finder.

## Discussion

You can safely call this method from any thread of your app.

## See Also

### Manipulating Files

func duplicate([URL], completionHandler: (([URL : URL], (any Error)?) -> Void)?)

Duplicates the specified URLS asynchronously in the same manner as the Finder.

func recycle([URL], completionHandler: (([URL : URL], (any Error)?) -> Void)?)

Moves the specified URLs to the trash in the same manner as the Finder.

func selectFile(String?, inFileViewerRootedAtPath: String) -> Bool

Selects the file at the specified path.

