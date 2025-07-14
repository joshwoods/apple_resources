

- Message UI
-  MFMailComposeResult 

Enumeration

# MFMailComposeResult

Result codes returned when the mail composition interface is dismissed.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum MFMailComposeResult
```

## Topics

### Constants

case cancelled

The user canceled the operation.

case saved

The email message was saved in the user’s drafts folder.

case sent

The email message was queued in the user’s outbox.

case failed

The email message was not saved or queued, possibly due to an error.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Responding to Email Completion

func mailComposeController(MFMailComposeViewController, didFinishWith: MFMailComposeResult, error: (any Error)?)

Tells the delegate that the user wants to dismiss the mail composition view.

**Required**

