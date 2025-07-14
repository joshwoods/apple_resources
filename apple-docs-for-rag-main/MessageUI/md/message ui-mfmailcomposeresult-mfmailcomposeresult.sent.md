

- Message UI
- MFMailComposeResult
-  MFMailComposeResult.sent 

Case

# MFMailComposeResult.sent

The email message was queued in the user’s outbox.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case sent
```

## Discussion

It is ready to send the next time the user connects to email.

## See Also

### Constants

case cancelled

The user canceled the operation.

case saved

The email message was saved in the user’s drafts folder.

case failed

The email message was not saved or queued, possibly due to an error.

