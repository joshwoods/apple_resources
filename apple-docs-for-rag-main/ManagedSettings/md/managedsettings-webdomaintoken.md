

- ManagedSettings
-  WebDomainToken 

Type Alias

# WebDomainToken

A representation of a web domain that preserves the user’s privacy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
typealias WebDomainToken = Token
```

## Discussion

Managed Settings uses representations of web domains to preserve user privacy and control. Use a token to represent a web domain without revealing what domain the token represents. FamilyActivitySelection provides tokens that devices within the same Family Sharing group can use to identify applications.

## See Also

### Websites

struct WebDomain

An object that represents a website.

