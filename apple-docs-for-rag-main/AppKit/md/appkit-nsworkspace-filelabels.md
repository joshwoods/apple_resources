

- AppKit
- NSWorkspace
-  fileLabels 

Instance Property

# fileLabels

The array of file labels, returned as strings.

macOS 10.6+

``` source
var fileLabels: [String] { get }
```

## Return Value

An array of strings.

## Discussion

You can listen for notifications named didChangeFileLabelsNotification to be notified when file labels change.

You can safely call this method from any thread of your app.

## See Also

### Finder File Labels

var fileLabelColors: [NSColor]

The array of colors for the file labels.

