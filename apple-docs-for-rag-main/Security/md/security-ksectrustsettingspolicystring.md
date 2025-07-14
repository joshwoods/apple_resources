

- Security
-  kSecTrustSettingsPolicyString 

Global Variable

# kSecTrustSettingsPolicyString

A string containing policy-specific data.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kSecTrustSettingsPolicyString: String { get }
```

## Discussion

The value is a CFString object. For the SMIME policy, this string contains an email address. For the SSL policy, it contains a host name.

