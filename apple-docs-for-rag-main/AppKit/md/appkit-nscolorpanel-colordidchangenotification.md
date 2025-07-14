

- AppKit
- NSColorPanel
-  colorDidChangeNotification 

Type Property

# colorDidChangeNotification

Posted when the color of the `NSColorPanel` is set, as when NSColorPanel is invoked.

macOS

``` source
class let colorDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the notifying `NSColorPanel`. This notification does not contain a `userInfo` dictionary.

## See Also

### Responding to a Color Change

protocol NSColorChanging

