

- AppKit
- NSScreen
-  colorSpaceDidChangeNotification 

Type Property

# colorSpaceDidChangeNotification

Posted when the color space of the screen has changed.

macOS 10.6+

``` source
class let colorSpaceDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the NSScreen object whose colorSpace has changed.. This notification does not contain a `userInfo` dictionary.

