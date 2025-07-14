

- Foundation
- NSNotification
- NSNotification.Name
-  MFMessageComposeViewControllerTextMessageAvailabilityDidChange 

Type Property

# MFMessageComposeViewControllerTextMessageAvailabilityDidChange

Posted when the value returned by the canSendText() class method has changed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static let MFMessageComposeViewControllerTextMessageAvailabilityDidChange: NSNotification.Name
```

## Discussion

Upon receiving this notification, query its `userInfo` dictionary with the MFMessageComposeViewControllerTextMessageAvailabilityKey key. If the availability of text message sending has changed, your app should invalidate caches and update its user interface as appropriate.

## See Also

### MessageUI

MFMessageComposeViewControllerTextMessageAvailabilityDidChangeNotification

Posted when the value returned by the class method has changed.

