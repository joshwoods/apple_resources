

- Bundle Resources
- Information Property List
-  NSIncludesSubdomains 

Property List Key

# NSIncludesSubdomains

A Boolean value that indicates whether to extend the configuration to subdomains of the given domain.

iOS 9.0+iPadOS 9.0+macOS 10.11+visionOS 1.0+

## Details 

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

You can include this key in any of the domain-specific dictionaries that you add to the NSExceptionDomains and NSPinnedDomains dictionaries. Adding the NSIncludesSubdomains key affects the applicability of the other configuration in the same domain-specific dictionary. The key is optional, with a default value of `NO`.

Set the value for this key to `YES` to apply the configuration for the given domain to all subdomains of the domain that have one additional path component. For example, if you set this value to `YES` and the domain name string is `example.com`, then the configuration applies to `example.com`, as well as `math.example.com` and `history.example.com`. However, it doesn’t apply to the subdomains `advanced.math.example.com` or `ancient.history.example.com` because those subdomains have two additional path components. If the value is `NO` the configuration applies only to `example.com`.

If you create an NSExceptionDomains dictionary for an IP address or a range of addresses, the NSIncludesSubdomains key has no effect for that exception.

## See Also

### Related Documentation

NSExceptionDomains

Custom App Transport Security (ATS) configurations for named domains.

**Name:** Exception Domains

NSPinnedDomains

A collection of certificates that App Transport Security expects when connecting to named domains.

