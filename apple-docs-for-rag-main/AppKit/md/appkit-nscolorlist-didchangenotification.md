

- AppKit
- NSColorList
-  didChangeNotification 

Type Property

# didChangeNotification

Posted whenever a color list changes.

macOS

``` source
class let didChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the NSColorList object that changed. This notification does not contain a `userInfo` dictionary.

