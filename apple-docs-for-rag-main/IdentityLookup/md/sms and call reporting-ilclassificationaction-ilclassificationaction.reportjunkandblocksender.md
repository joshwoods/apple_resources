

- SMS and Call Reporting
- ILClassificationAction
-  ILClassificationAction.reportJunkAndBlockSender 

Case

# ILClassificationAction.reportJunkAndBlockSender

The system should report the communication as junk and add the number to the system’s block list.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
case reportJunkAndBlockSender
```

## Discussion

The extension creates an SMS message based on the response, and displays the message to the user. The user can then send or cancel the report.

Next, the extension displays an alert to notify the user that the number will be blocked. To unblock the number, users must go to the Call Blocking & Identification settings in the Settings app.

Finally, the extension dismisses the ILClassificationUIExtensionViewController.

## See Also

### Classifications

case none

No action is required.

case reportJunk

The system should report the communication as junk.

case reportNotJunk

The system should report that the communication is not junk.

