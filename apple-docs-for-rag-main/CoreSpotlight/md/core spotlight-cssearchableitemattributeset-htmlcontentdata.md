

- Core Spotlight
- CSSearchableItemAttributeSet
-  htmlContentData 

Instance Property

# htmlContentData

The HTML content of the document encoded as an NSData object representing a UTF-8 encoded string.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var htmlContentData: Data? { get set }
```

## See Also

### Describing messages

Common Mailbox Identifiers

Constants that describe common mailbox names.

var accountHandles: [String]?

An array of the canonical handles for the account with which the message is associated.

var accountIdentifier: String?

The unique identifier for the account with which the message is associated, if any.

var additionalRecipients: [CSPerson]?

An array of CSPerson objects representing the content of the Cc: field in an email message.

var authorAddresses: [String]?

An array of addresses associated with the author of the message.

var authorEmailAddresses: [String]?

An array of email addresses associated with the author of the message.

var authorNames: [String]?

An array of names representing the authors who have worked on the message.

var authors: [CSPerson]?

An array of CSPerson objects representing the content of the From: field in an item.

var emailAddresses: [String]?

An array of email addresses associated with the message.

var emailHeaders: [String : [Any]]?

A dictionary that contains all the headers of the message.

var hiddenAdditionalRecipients: [CSPerson]?

An array of CSPerson objects representing the content of the Bcc: field in an email message.

var instantMessageAddresses: [String]?

An array of instant message addresses for the message.

var likelyJunk: NSNumber

A value that indicates if the message is likely to be considered junk.

var mailboxIdentifiers: [String]?

An array of mailbox identifiers associated with the message.

var phoneNumbers: [String]?

An array of phone numbers associated with the message.

