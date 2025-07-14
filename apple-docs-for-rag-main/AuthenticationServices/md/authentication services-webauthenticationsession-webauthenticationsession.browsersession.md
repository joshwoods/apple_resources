

- Authentication Services
- WebAuthenticationSession
-  WebAuthenticationSession.BrowserSession 

Structure

# WebAuthenticationSession.BrowserSession

Describes the preferred browser session behavior.

AuthenticationServicesSwiftUIiOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
struct BrowserSession
```

## Topics

### Behaviors

static var ephemeral: WebAuthenticationSession.BrowserSession

A session that doesn’t share cookies or other browsing data with a person’s normal browser session.

static var shared: WebAuthenticationSession.BrowserSession

A session that can share cookies and other browsing data with a person’s normal browser session.

## Relationships

### Conforms To

- Sendable

## See Also

### Authenticating a session

func authenticate(using: URL, callbackURLScheme: String, preferredBrowserSession: WebAuthenticationSession.BrowserSession?) async throws -> URL

Begins a web authentication session.

Deprecated

