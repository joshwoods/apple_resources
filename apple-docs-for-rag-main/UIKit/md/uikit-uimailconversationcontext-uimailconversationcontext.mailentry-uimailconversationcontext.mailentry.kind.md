

- UIKit
- UIMailConversationContext
- UIMailConversationContext.MailEntry
-  UIMailConversationContext.MailEntry.Kind 

Enumeration

# UIMailConversationContext.MailEntry.Kind

A set of categories for an email.

iOS 18.4+iPadOS 18.4+

``` source
enum Kind
```

## Topics

### Kinds of email

case news

The email is related to news or current events.

case none

The email does not fit in a specific category.

case personal

The email is personal correspondence.

case promotion

The email contains a promotional offer.

case social

The email is related to social media.

case transaction

The email is related to a purchase or transaction.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Categorizing the email

var kind: UIMailConversationContext.MailEntry.Kind

An item that reflects the category that describes an email.

