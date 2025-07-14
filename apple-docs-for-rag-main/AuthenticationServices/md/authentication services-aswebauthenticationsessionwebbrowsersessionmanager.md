

- Authentication Services
-  ASWebAuthenticationSessionWebBrowserSessionManager 

Class

# ASWebAuthenticationSessionWebBrowserSessionManager

A session manager that mediates sharing data between an app and a web browser.

macOS 10.15+

``` source
class ASWebAuthenticationSessionWebBrowserSessionManager
```

## Overview

You don’t create a session manager directly. Instead, use the shared session manager to tell the system what instance within your web browser app handles authentication requests. Do this by assigning an instance of a class that adopts the ASWebAuthenticationSessionWebBrowserSessionHandling protocol to the shared manager’s sessionHandler property.

You can also use the shared managers wasLaunchedByAuthenticationServices property to determine if your web browser app was launched for the specific purpose of performing authentication.

## Topics

### Getting the Shared Manager

class var shared: ASWebAuthenticationSessionWebBrowserSessionManager

The shared manager for which a web browser acts as the session handler.

### Handling a Session Request

var sessionHandler: any ASWebAuthenticationSessionWebBrowserSessionHandling

A handler that a web browser provides to handle session requests from an app.

protocol ASWebAuthenticationSessionWebBrowserSessionHandling

An interface that a session handler implements to handle login requests from an app.

### Querying the Manager

var wasLaunchedByAuthenticationServices: Bool

A Boolean that indicates whether the session was launched by authentication services.

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

### Web authentication sessions

Authenticating a User Through a Web Service

Use a web authentication session to authenticate a user in your app.

Securing Logins with iCloud Keychain Verification Codes

Use time-based codes generated on-device for a secure authentication experience.

class ASWebAuthenticationSession

A session that an app uses to authenticate a user through a web service.

struct WebAuthenticationSession

A SwiftUI environment value that views use to authenticate someone using a web service.

Supporting Single Sign-On in a Web Browser App

Extend your web browser app to handle web authentication requests from other apps.

ASWebAuthenticationSessionWebBrowserSupportCapabilities

A collection of keys that a browser app uses to declare its ability to handle authentication requests from other apps.

