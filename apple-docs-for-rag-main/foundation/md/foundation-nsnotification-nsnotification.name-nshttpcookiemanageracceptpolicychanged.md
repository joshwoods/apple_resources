

- Foundation
- NSNotification
- NSNotification.Name
-  NSHTTPCookieManagerAcceptPolicyChanged 

Type Property

# NSHTTPCookieManagerAcceptPolicyChanged

A notification posted when the acceptance policy of the cookie storage has changed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSHTTPCookieManagerAcceptPolicyChanged: NSNotification.Name
```

## Discussion

In macOS, cookies are shared among applications, meaning this notification can be received as a result of another application’s actions. Cookies are not shared among applications in iOS.

The notification’s object is the HTTPCookieStorage instance. This notification does not contain a userInfo dictionary.

## See Also

### Tracking cookie storage changes

static let NSHTTPCookieManagerCookiesChanged: NSNotification.Name

A notification posted when the cookies stored in the cookie storage have changed.

