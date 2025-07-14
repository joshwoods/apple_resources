

- Message UI
-  MFMessageComposeViewControllerTextMessageAvailabilityKey 

Global Variable

# MFMessageComposeViewControllerTextMessageAvailabilityKey

The value of this key is a number object that contains a Boolean value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
let MFMessageComposeViewControllerTextMessageAvailabilityKey: String
```

## Discussion

This value matches the result of the canSendText() class method.The `userInfo` dictionary for the MFMessageComposeViewControllerTextMessageAvailabilityDidChange notification includes this key. The value of this key is an NSNumber object that contains a Boolean value. This value matches the result of the canSendText() class method.

## See Also

### Handling notifications

static let MFMessageComposeViewControllerTextMessageAvailabilityDidChange: NSNotification.Name

Posted when the value returned by the class method has changed.

