

- Network Extension
- NEFilterProviderConfiguration
-  organization 

Instance Property

# organization

A string that identifies the organization that administers the filter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var organization: String? { get set }
```

## See Also

### Accessing the filter configuration

var vendorConfiguration: [String : Any]?

A dictionary of provider-specific configuration settings.

var serverAddress: String?

The address of a server that the Filter Control Provider may contact for rules and other configuration information.

var username: String?

A string that identifies the user.

var passwordReference: Data?

A persistent reference to a keychain item containing a password associated with the filter.

var identityReference: Data?

A persistent reference to a keychain item containing a certificate and private key associated with the filter.

