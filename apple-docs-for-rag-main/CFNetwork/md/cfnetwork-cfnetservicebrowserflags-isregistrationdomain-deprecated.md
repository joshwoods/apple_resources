

- CFNetwork
- CFNetServiceBrowserFlags
-  isRegistrationDomain Deprecated

Type Property

# isRegistrationDomain

tvOS 9.0+visionOS 1.0–1.0Deprecated

``` source
static var isRegistrationDomain: CFNetServiceBrowserFlags { get }
```

Deprecated

Use isDefault instead.

## See Also

### Type Properties

static var isDefault: CFNetServiceBrowserFlags

Specifies whether the resulting domain is the default registration or browse domain.

static var isDomain: CFNetServiceBrowserFlags

Specifies whether the result pertains to a search for domains or services.

static var moreComing: CFNetServiceBrowserFlags

A hint that the system will call the client’s callback function again soon.

static var remove: CFNetServiceBrowserFlags

Specifies whether the client should remove the result instead of adding it.

