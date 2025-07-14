

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
- CredentialSession.Credential.InstanceInfo
-  securityDomainKeyInfo 

Instance Property

# securityDomainKeyInfo

A data blob which contains the security domain On-Board Generated Key (OBGK).

iOS 18.1+iPadOS 18.1+

``` source
let securityDomainKeyInfo: Data
```

## Discussion

This data has the information required to form a Secure Channel Protocol 3 (SCP03) channel between the user and the security domain.

## See Also

### Creating a secure channel

let securityDomainAID: Data

The unique identifier of the security domain you use to install the instance.

