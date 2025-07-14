

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
- CredentialSession.Credential.InstanceInfo
-  securityDomainAID 

Instance Property

# securityDomainAID

The unique identifier of the security domain you use to install the instance.

iOS 18.1+iPadOS 18.1+

``` source
let securityDomainAID: Data
```

## Discussion

Use this identifier when selecting the security domain to perform data transceive with, such as forming a Secure Channel Protocol 3 (SCP03) channel.

## See Also

### Creating a secure channel

let securityDomainKeyInfo: Data

A data blob which contains the security domain On-Board Generated Key (OBGK).

