

- MarketplaceKit
- AppLibrary
-  requestAppInstallationFromBrowser(for:referrer:) 

Instance Method

# requestAppInstallationFromBrowser(for:referrer:)

Forwards an app installation request from the developer’s webpage.

iOS 17.4+iPadOS 17.4+

``` source
nonisolated
final func requestAppInstallationFromBrowser(
    for url: URL,
    referrer: URL
) async throws
```

## Parameters 

`url`  

The unparsed `marketplace-kit` URL that triggers the installation request.

`referrer`  

The origin of the top frame that contains the alternative marketplace installation URL.

## Mentioned in 

Enabling alternative distribution app installation in a browser

## Discussion

Web browsers that render with BrowserEngineKit rather than WebKit call this method to forward the installation of an app from the developer’s webpage. Your browser listens for MarketplaceKitURIScheme invocations to field such requests.

For more information, see Enabling alternative distribution app installation in a browser.

