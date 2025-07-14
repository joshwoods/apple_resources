

- Authentication Services
- ASWebAuthenticationSession
-  init(url:callbackURLScheme:completionHandler:) Deprecated

Initializer

# init(url:callbackURLScheme:completionHandler:)

Creates a web authentication session instance.

iOS 12.0–18.4DeprecatediPadOS 12.0–18.4DeprecatedMac Catalyst 12.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 16.0–18.4DeprecatedvisionOS 1.0+watchOS 6.2–11.4Deprecated

``` source
init(
    url URL: URL,
    callbackURLScheme: String?,
    completionHandler: @escaping ASWebAuthenticationSession.CompletionHandler
)
```

Deprecated

Use initWithURL:callback:completionHandler: instead

## Parameters 

`URL`  

A URL with the `http` or `https` scheme pointing to the authentication webpage.

`callbackURLScheme`  

The custom URL scheme that the app expects in the callback URL.

`completionHandler`  

A completion handler the session calls when it completes successfully, or when the user cancels the session.

## See Also

### Creating a Session

typealias CompletionHandler

A completion handler for the web authentication session.

