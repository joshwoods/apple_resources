

- AppKit
- NSWorkspace
-  selectFile(\_:inFileViewerRootedAtPath:) 

Instance Method

# selectFile(\_:inFileViewerRootedAtPath:)

Selects the file at the specified path.

macOS

``` source
func selectFile(
    _ fullPath: String?,
    inFileViewerRootedAtPath rootFullPath: String
) -> Bool
```

## Parameters 

`fullPath`  

The full path of the file to select.

`rootFullPath`  

The path to use for the file viewer. If you specify a nonempty path string, this method opens a new file viewer. If you specify an empty string (`@""`), this method selects the file in the main viewer.

## Return Value

true if the file was successfully selected; otherwise, false.

## Discussion

In macOS 10.5 and later, this method does not follow symlinks when selecting the file. If the `fullPath` parameter contains any symlinks, this method selects the symlink instead of the file it targets. If you want to select the target file, use the resolvingSymlinksInPath method to resolve any symlinks before calling this method.

You can safely call this method from any thread of your app.

## See Also

### Manipulating Files

func duplicate([URL], completionHandler: (([URL : URL], (any Error)?) -> Void)?)

Duplicates the specified URLS asynchronously in the same manner as the Finder.

func recycle([URL], completionHandler: (([URL : URL], (any Error)?) -> Void)?)

Moves the specified URLs to the trash in the same manner as the Finder.

func activateFileViewerSelecting([URL])

Activates the Finder, and opens one or more windows selecting the specified files.

