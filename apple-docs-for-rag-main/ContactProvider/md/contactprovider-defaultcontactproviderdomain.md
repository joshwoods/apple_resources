

- ContactProvider
-  DefaultContactProviderDomain 

Structure

# DefaultContactProviderDomain

The default domain the extension uses.

iOS 18.0+iPadOS 18.0+

``` source
struct DefaultContactProviderDomain
```

## Topics

### Creating a default domain

init()

Creates an instance of the default domain.

### Identifying the domain

let displayName: String

The display name the system shows to represent the default domain.

var identifier: String

The identifier of the domain.

### Providing custom domain data

let userInfo: Dictionary&lt;String, Any>

Custom values used to configure the extension before enumeration begins.

### Using the default domain identifier

static let identifier: String

The identifier used for all default domains.

## Relationships

### Conforms To

- ContactProviderDomain

## See Also

### Working with domains

protocol ContactProviderDomain

A domain, including traits like an identifier and display name, used to configure the extension.

