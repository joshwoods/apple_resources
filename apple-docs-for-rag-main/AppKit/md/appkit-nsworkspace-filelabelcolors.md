

- AppKit
- NSWorkspace
-  fileLabelColors 

Instance Property

# fileLabelColors

The array of colors for the file labels.

macOS 10.6+

``` source
var fileLabelColors: [NSColor] { get }
```

## Return Value

An array of `NSColor` objects.

## Discussion

This array has the same number of elements as fileLabels, and the color at a given index corresponds to the label at the same index.

You can listen for notifications named didChangeFileLabelsNotification to be notified when file labels change that may result in changes to the order of the `fileLabelColors`.

You can safely call this method from any thread of your app.

## See Also

### Finder File Labels

var fileLabels: [String]

The array of file labels, returned as strings.

