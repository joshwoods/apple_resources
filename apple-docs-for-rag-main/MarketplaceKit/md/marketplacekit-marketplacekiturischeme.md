

- MarketplaceKit
-  MarketplaceKitURIScheme 

Global Variable

# MarketplaceKitURIScheme

A URI scheme that defines an alternative distribution app installation link.

iOS 17.4+iPadOS 17.4+

``` source
let MarketplaceKitURIScheme: String
```

## Mentioned in 

Installing your app from your website

Enabling alternative distribution app installation in a browser

Distributing your app from your website

Installing apps from an alternative marketplace

Ingesting an alternative distribution package

## Discussion

This installation scheme defines how your webpage requests the installation of your app. For example, assign a URL with the following scheme to a Download button on your page:

```
marketplace-kit://install
    ?alternativeDistributionPackage=
    &installVerificationToken=    
    &token=
    &account=
    &appShareURL=;
```

The URL parameters are:

| URL parameter | Description |
|----|----|
| `alternativeDistributionPackage` | Your app’s alternative distribution package in the assembled format described in Ingesting an alternative distribution package. |
| `installVerificationToken` | A required JSON web signature (JWS). For more information, see Supplying an install verification token. |
| `token` | An optional authentication token to include if downloads require authorization. iOS sends the token back to your token endpoint to reference this request. The value is free-form, and can contain any information at your discretion, such as an id that identifies the customer. |
| `account` | An optional user ID for the page visitor. iOS groups apps in restore requests based on `account`. iOS also provides the `account` as `login_hint` for the authorization call during interactive re-authentication; for more information, see Reauthenticating a person to manage apps. |
| `appShareURL` | An optional URL to a product landing page for the app on your marketplace website. The operating system populates the value in the Share Sheet when a person touches and holds the app’s icon on the Home Screen. |

Web browsers recognize the scheme and hand off the installation request to MarketplaceKit. For more information, see Installing your app from your website.

## Setting the alternative distribution package parameter

The fully qualified domain in the `alternateDistributionPackage` value needs to match the fully qualified domain of the *referrer*, that is, the page that contains the `marketplace-kit://` link. This domain also needs to match the domain you supply to App Store Connect. For more information, see Alternative Distribution Domains. For example:

Domain in App Store Connect  
`mydomain.com`

Your webpage root domain  
`mymarketplace.mydomain.com`

`alternateDistributionPackage` value  
`https://mymarketplace.mydomain.com/path`

Note

To allow installation, the web browser also needs to support the app installation URL scheme. If you develop a browser app, see Enabling alternative distribution app installation in a browser for more information.

## See Also

### App management

class AppLibrary

An object that manages search characteristics, licensing, and the installation of apps.

struct AppVersion

Information that describes an app, including its identifier and version number.

struct AutomaticUpdate

Information that describes an app that’s available for update, including a download URL.

struct InstallRequirements

An app’s installation criteria for a device.

typealias AppleItemID

An identifier that represents an app.

typealias AppleVersionID

An identifier that represents a single app version.

