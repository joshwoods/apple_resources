

- UIKit
- UIMailConversationContext
-  responseHasCustomSignature 

Instance Property

# responseHasCustomSignature

A Boolean value that indicates whether the intended response contains a custom signature.

iOS 18.4+iPadOS 18.4+

``` source
var responseHasCustomSignature: Bool { get set }
```

## See Also

### Getting message details

var responseSubject: String

A string that contains the subject line of an intended response.

var responseSecondaryRecipientIdentifiers: Set&lt;String>

A set of strings that identifies the secondary recipients of the message, such as those in CC or BCC messages.

