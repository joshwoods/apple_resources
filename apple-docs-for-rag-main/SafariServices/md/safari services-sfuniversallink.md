

- Safari Services
-  SFUniversalLink 

Class

# SFUniversalLink

An object that provides browsers with the ability to discover associations between an app and a website.

macOS 10.15+

``` source
class SFUniversalLink
```

## Overview

Universal links are a bridge between an app and a website that have related content, such as products or services. Typically, clicking a link in a browser takes a person to a website. However, the person may have an app that provides the same content and a better experience.

A web browser uses the `SFUniversalLink` class to discover such applications and provide the person with additional options for interaction beyond the default browser behavior.

In order to use universal links, you need to use the entitlement com.apple.developer.associated-domains.applinks.read-write with a value of `true`. Before you submit an app with the entitlement to the App Store, you need to get permission to use the entitlement. Request permission at https://developer.apple.com/contact/request/browser-universal-links-request.

## Topics

### Initializing a Link

init?(webpageURL: URL)

Creates a universal link object with the URL.

### Configuring Universal Links

var applicationURL: URL

The URL to the app that can open this universal link.

var isEnabled: Bool

A flag that indicates whether the universal link is enabled.

var webpageURL: URL

The URL specified when initializing the receiver.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Associated domains

Supporting associated domains

Connect your app and a website to provide both a native app and a browser experience.

Associated Domains Entitlement

The associated domains for specific services, such as shared web credentials, universal links, and App Clips.

