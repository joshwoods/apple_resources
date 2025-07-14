

- Security
- SecTrustResultType
-  SecTrustResultType.deny 

Case

# SecTrustResultType.deny

The user specified that the certificate should not be trusted.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case deny
```

## Discussion

This value indicates that the user explicitly chose to not trust a certificate in the chain, usually by clicking the appropriate button in a certificate trust panel. Your app should *not* trust the chain. The Keychain Access utility refers to this value as “Never Trust.”

