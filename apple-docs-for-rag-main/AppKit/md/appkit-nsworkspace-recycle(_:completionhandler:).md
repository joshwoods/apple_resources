

- AppKit
- NSWorkspace
-  recycle(\_:completionHandler:) 

Instance Method

# recycle(\_:completionHandler:)

Moves the specified URLs to the trash in the same manner as the Finder.

macOS 10.6+

``` source
func recycle(
    _ URLs: [URL],
    completionHandler handler: (([URL : URL], (any Error)?) -> Void)? = nil
)
```

``` source
func recycle(_ URLs: [URL]) async throws -> [URL : URL]
```

## Parameters 

`URLs`  

An array of NSURL objects representing the files to move to the trash. This parameter must not be `nil`

`handler`  

The completion handler block object to call when the operation completes. You may specify `nil` for this parameter. If this parameter is not `nil`, you must call the recycle(_:completionHandler:) method from a block running on an active dispatch queue; your completion handler block is subsequently executed on the same dispatch queue.

The block takes two arguments:

newURLs  
A dictionary that maps the file’s original location to its location in the trash. Each key is a URL from the `URLs` parameter. The value of each key is a URL representing the location of the file in the trash. If this method could not move a file to the trash, the corresponding URL is not included in the dictionary.

error  
If the operation succeeded for every file, this parameter is `nil`. If the operation failed for one or more files, the parameter contains an error object describing the overall result of the operation in a manner suitable for presentation to the user.

## Discussion

This method may cause a progress indicator, or other user interface element, to be shown by the Finder.

In macOS 10.6, this method requires the app to run the main run loop in a common mode to facilitate the display of any user interface elements. You can safely call this method from any thread of your app.

## See Also

### Manipulating Files

func duplicate([URL], completionHandler: (([URL : URL], (any Error)?) -> Void)?)

Duplicates the specified URLS asynchronously in the same manner as the Finder.

func activateFileViewerSelecting([URL])

Activates the Finder, and opens one or more windows selecting the specified files.

func selectFile(String?, inFileViewerRootedAtPath: String) -> Bool

Selects the file at the specified path.

