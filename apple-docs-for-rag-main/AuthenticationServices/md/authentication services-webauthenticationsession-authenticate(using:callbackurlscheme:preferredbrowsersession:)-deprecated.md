

- Authentication Services
- WebAuthenticationSession
-  authenticate(using:callbackURLScheme:preferredBrowserSession:) Deprecated

Instance Method

# authenticate(using:callbackURLScheme:preferredBrowserSession:)

Begins a web authentication session.

AuthenticationServicesSwiftUIiOS 16.4–18.4DeprecatediPadOS 16.4–18.4DeprecatedMac Catalyst 16.4–18.4DeprecatedmacOS 13.3–15.4DeprecatedtvOS 16.4–18.4DeprecatedvisionOS 1.0+watchOS 9.4–11.4Deprecated

``` source
@MainActor
func authenticate(
    using url: URL,
    callbackURLScheme: String,
    preferredBrowserSession: WebAuthenticationSession.BrowserSession? = nil
) async throws -> URL
```

Deprecated

Use \`authenticate(using:callback:preferredBrowserSession:additionalHeaderFields:)\` instead

## Parameters 

`url`  

A URL beginning with HTTP or HTTPS that points to the authentication webpage.

`callbackURLScheme`  

The app’s custom callback scheme.

`preferredBrowserSession`  

The preferred data-sharing behavior of the browser session. For more information, see WebAuthenticationSession.BrowserSession.

## Return Value

The URL that the authentication provider returns.

## See Also

### Authenticating a session

struct BrowserSession

Describes the preferred browser session behavior.

