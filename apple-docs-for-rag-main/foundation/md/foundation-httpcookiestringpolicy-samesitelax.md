

- Foundation
- HTTPCookieStringPolicy
-  sameSiteLax 

Type Property

# sameSiteLax

A policy that allows certain cross-site requests to include the cookie.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let sameSiteLax: HTTPCookieStringPolicy
```

## Discussion

When a cookie has this policy, a request includes the cookie if the request is “top-level,”, meaning one that changes the URL in the address bar.

## See Also

### Policies

static let sameSiteStrict: HTTPCookieStringPolicy

A policy that prohibits a cross-site request from including the cookie.

