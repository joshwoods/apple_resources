

- SecureElementCredential
- CredentialSession
-  configuration() 

Instance Method

# configuration()

Retrieves a transaction configuration related to this session.

SecureElementCredentialSwiftUIiOS 18.1+iPadOS 18.1+

``` source
nonisolated
func configuration() async throws -> CredentialTransaction.Configuration
```

## Discussion

This method provides a way to get the session configuration after performing a transaction task with a SwiftUI view.

Clients should call invalidate() on this configuration after completing each transaction.

Warning

Don’t import UIKit in any file that imports this type. This causes ambiguity resolving the SecureElementCredential framework’s SwiftUI and UIKit symbols.

## See Also

### Using SwiftUI

class Configuration

An object that provides configuration information for a transaction that the client intends to peform.

