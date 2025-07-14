

- AppKit
- NSBrowser
-  columnConfigurationDidChangeNotification 

Type Property

# columnConfigurationDidChangeNotification

Notifies the delegate when the width of a browser column has changed.

macOS

``` source
class let columnConfigurationDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the browser whose column sizes need to be made persistent. This notification does not contain a `userInfo` dictionary. If the user resizes more than one column, a single notification is posted when the user is finished resizing.

## See Also

### Related Documentation

func browserColumnConfigurationDidChange(Notification)

Used by clients to implement their own column width persistence.

