

- Foundation
- NSNotification
- NSNotification.Name
-  NSClassDescriptionNeededForClass 

Type Property

# NSClassDescriptionNeededForClass

Posted by init(for:) when a class description cannot be found for a class.

Mac Catalyst 13.0+macOS 10.0+

``` source
static let NSClassDescriptionNeededForClass: NSNotification.Name
```

## Discussion

After the notification is processed, init(for:) checks for a class description again. This checking allows an observer to register class descriptions lazily. The notification is posted only once for any given class, even if the class description remains undefined.

The notification object is the class object for which the class description is requested. This notification does not contain a `userInfo` dictionary.

