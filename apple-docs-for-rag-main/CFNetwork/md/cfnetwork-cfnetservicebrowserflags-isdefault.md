

- CFNetwork
- CFNetServiceBrowserFlags
-  isDefault 

Type Property

# isDefault

Specifies whether the resulting domain is the default registration or browse domain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
static var isDefault: CFNetServiceBrowserFlags { get }
```

## Discussion

If set, the resulting domain is the default registration or browse domain, depending on the context. For this version of the CFNetServices API, the default registration domain is the local domain.

Note

In previous versions of this API, this constant was `kCFNetServiceFlagIsRegistrationDomain`, which is retained for backward compatibility.

## See Also

### Type Properties

static var isDomain: CFNetServiceBrowserFlags

Specifies whether the result pertains to a search for domains or services.

static var isRegistrationDomain: CFNetServiceBrowserFlagsDeprecated

static var moreComing: CFNetServiceBrowserFlags

A hint that the system will call the client’s callback function again soon.

static var remove: CFNetServiceBrowserFlags

Specifies whether the client should remove the result instead of adding it.

static var isRegistrationDomain: CFNetServiceBrowserFlagsDeprecated

