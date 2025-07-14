

- SecureElementCredential
- CredentialSession
- CredentialSession.ErrorCode
-  CredentialSession.ErrorCode.network 

Case

# CredentialSession.ErrorCode.network

The device’s internet connection is offline.

iOS 18.1+iPadOS 18.1+

``` source
case network
```

## Discussion

Your app can try again after receiving this error, to see if network communication is restored.

