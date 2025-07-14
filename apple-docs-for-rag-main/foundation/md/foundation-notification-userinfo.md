

- Foundation
- Notification
-  userInfo 

Instance Property

# userInfo

Storage for values or objects related to this notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var userInfo: [AnyHashable : Any]?
```

## Discussion

The user information dictionary stores any additional objects that objects receiving the notification might use.

For example, in AppKit, NSControl objects post the textDidChangeNotification whenever the field editor (an NSText object) changes text inside the `NSControl`. This notification provides the `NSControl` object as the notification’s associated object. In order to provide access to the field editor, the `NSControl` object posting the notification adds the field editor to the notification’s user information dictionary. Objects receiving the notification can access the field editor and the `NSControl` object posting the notification as follows:

```
func controlTextDidChange(_ notification: Notification) 
{
    if let fieldEditor = notification.userInfo?["NSFieldEditor"] as? NSText,
        let postingObject = notification.object as? NSControl
    {
        // work with the field editor and posting object
    }
}
```

## See Also

### Getting Notification Information

var name: Notification.Name

A tag identifying the notification.

var object: Any?

An object that the poster wishes to send to observers.

