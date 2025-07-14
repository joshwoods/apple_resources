

- AppKit
- NSImageRep
-  registryDidChangeNotification 

Type Property

# registryDidChangeNotification

Posted whenever the image representation class registry changes.

macOS

``` source
class let registryDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the image class that is registered or unregistered. This notification does not contain a `userInfo` dictionary.

