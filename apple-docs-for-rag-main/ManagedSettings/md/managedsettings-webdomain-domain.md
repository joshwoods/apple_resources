

- ManagedSettings
- WebDomain
-  domain 

Instance Property

# domain

A string that identifies a specific web domain.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
let domain: String?
```

## Discussion

In an extension that provides shield configurations, this property provides the web domain. When you access this property outside that extension, the value is `nil`. See ShieldConfigurationDataSource for more information.

## See Also

### Identifying a Web Domain

let token: WebDomainToken?

An opaque representation of a specific web domain.

