

- AppKit
- NSColorSampler
-  show(selectionHandler:) 

Instance Method

# show(selectionHandler:)

Displays the system color-sampling interface asynchronously and reports the selected color back to your app.

macOS 10.15+

``` source
func show(selectionHandler: @escaping (NSColor?) -> Void)
```

``` source
func sample() async -> NSColor?
```

## Parameters 

`selectionHandler`  

The handler block for processing the user-selected color. AppKit calls this block on your app’s main thread. This block has no return value and takes the following parameter:

selectedColor  
The selected color.

## Discussion

This method displays the color-sampling interface and returns immediately. The color-sampling interface magnifies the onscreen pixels and makes it easier for the user to select a single pixel. When the user clicks any mouse button, AppKit dismisses the interface and calls `selectionHandler` with the results.

