

- Foundation
- NSNotification
- NSNotification.Name
-  NSHTTPCookieManagerCookiesChanged 

Type Property

# NSHTTPCookieManagerCookiesChanged

A notification posted when the cookies stored in the cookie storage have changed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSHTTPCookieManagerCookiesChanged: NSNotification.Name
```

## Discussion

The notification’s object is the HTTPCookieStorage instance. This notification does not contain a userInfo dictionary.

## See Also

### Tracking cookie storage changes

static let NSHTTPCookieManagerAcceptPolicyChanged: NSNotification.Name

A notification posted when the acceptance policy of the cookie storage has changed.

