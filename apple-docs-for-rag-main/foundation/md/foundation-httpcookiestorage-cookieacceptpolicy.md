

- Foundation
- HTTPCookieStorage
-  cookieAcceptPolicy 

Instance Property

# cookieAcceptPolicy

The cookie storage’s cookie accept policy.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var cookieAcceptPolicy: HTTPCookie.AcceptPolicy { get set }
```

## Discussion

The default cookie accept policy is HTTPCookie.AcceptPolicy.always. Changing the cookie policy affects all currently running applications using the cookie storage.

## See Also

### Getting and setting the cookie accept policy

enum AcceptPolicy

Cookie acceptance policies implemented by the HTTPCookieStorage class.

