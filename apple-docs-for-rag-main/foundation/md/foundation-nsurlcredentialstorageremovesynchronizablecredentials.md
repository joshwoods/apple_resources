

- Foundation
-  NSURLCredentialStorageRemoveSynchronizableCredentials 

Global Variable

# NSURLCredentialStorageRemoveSynchronizableCredentials

The corresponding value is an `NSNumber` object representing a Boolean value that indicates whether credentials which contain the URLCredential.Persistence.synchronizable attribute should be removed.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSURLCredentialStorageRemoveSynchronizableCredentials: String
```

## Discussion

If the key is missing or the value is `@NO`, then no attempt will be made to remove such a credential.

