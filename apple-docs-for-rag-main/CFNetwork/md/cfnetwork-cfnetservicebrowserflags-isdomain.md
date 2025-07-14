

- CFNetwork
- CFNetServiceBrowserFlags
-  isDomain 

Type Property

# isDomain

Specifies whether the result pertains to a search for domains or services.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
static var isDomain: CFNetServiceBrowserFlags { get }
```

## Discussion

If set, the results pertain to a search for domains. If not set, the results pertain to a search for services.

## See Also

### Type Properties

static var isDefault: CFNetServiceBrowserFlags

Specifies whether the resulting domain is the default registration or browse domain.

static var isRegistrationDomain: CFNetServiceBrowserFlagsDeprecated

static var moreComing: CFNetServiceBrowserFlags

A hint that the system will call the client’s callback function again soon.

static var remove: CFNetServiceBrowserFlags

Specifies whether the client should remove the result instead of adding it.

static var isRegistrationDomain: CFNetServiceBrowserFlagsDeprecated

