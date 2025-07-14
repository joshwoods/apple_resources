

- ContactProvider
-  ContactProviderDomain 

Protocol

# ContactProviderDomain

A domain, including traits like an identifier and display name, used to configure the extension.

iOS 18.0+iPadOS 18.0+

``` source
protocol ContactProviderDomain
```

## Topics

### Identifying the domain

var displayName: String

The display name the system shows to represent this domain.

**Required**

var identifier: String

The identifier of the domain.

**Required**

### Providing custom domain data

var userInfo: Dictionary&lt;String, Any>

Custom values used to configure the extension before enumeration begins.

**Required**

## Relationships

### Conforming Types

- DefaultContactProviderDomain

## See Also

### Working with domains

struct DefaultContactProviderDomain

The default domain the extension uses.

