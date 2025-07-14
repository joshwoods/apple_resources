

- WebKit
- WKHTTPCookieStoreObserver
-  cookiesDidChange(in:) 

Instance Method

# cookiesDidChange(in:)

Tells the delegate that the cookies in the specified cookie store changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
optional func cookiesDidChange(in cookieStore: WKHTTPCookieStore)
```

## Parameters 

`cookieStore`  

The cookie store that contains the modified cookies.

## Discussion

When the value of a cookie changes, the cookie store calls this method on all registered observer objects. Use this method to fetch the new cookie values and update any app-specific data structures or JavaScript environment variables that use those values.

