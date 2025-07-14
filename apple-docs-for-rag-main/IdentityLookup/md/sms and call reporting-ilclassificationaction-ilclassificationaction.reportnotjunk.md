

- SMS and Call Reporting
- ILClassificationAction
-  ILClassificationAction.reportNotJunk 

Case

# ILClassificationAction.reportNotJunk

The system should report that the communication is not junk.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
case reportNotJunk
```

## Discussion

The extension creates an SMS message based on the response, and displays the message to the user. The user can then send or cancel the report. Finally, the extension dismisses the ILClassificationUIExtensionViewController.

## See Also

### Classifications

case none

No action is required.

case reportJunk

The system should report the communication as junk.

case reportJunkAndBlockSender

The system should report the communication as junk and add the number to the system’s block list.

