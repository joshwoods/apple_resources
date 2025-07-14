

- Authentication Services
- WebAuthenticationSession
-  authenticate(using:callback:preferredBrowserSession:additionalHeaderFields:) 

Instance Method

# authenticate(using:callback:preferredBrowserSession:additionalHeaderFields:)

AuthenticationServicesSwiftUIiOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
@MainActor
func authenticate(
    using url: URL,
    callback: ASWebAuthenticationSession.Callback,
    preferredBrowserSession: WebAuthenticationSession.BrowserSession? = nil,
    additionalHeaderFields: [String : String]
) async throws -> URL
```

