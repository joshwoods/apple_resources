

- WebKit
- WKHTTPCookieStore
-  getCookiePolicy(\_:) 

Instance Method

# getCookiePolicy(\_:)

Returns a cookie policy that indicates whether the cookie store allows cookie storage.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
func getCookiePolicy(_ completionHandler: @escaping @MainActor (WKHTTPCookieStore.CookiePolicy) -> Void)
```

``` source
@MainActor
var cookiePolicy: WKHTTPCookieStore.CookiePolicy { get async }
```

## Parameters 

`completionHandler`  

The completion handler block to execute asynchronously with the cookie policy. This block has no return value, and takes the following parameter:

cookiePolicy  
A WKHTTPCookieStore.CookiePolicy case that indicates whether the cookie store allows cookie storage.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
var cookiePolicy: WKHTTPCookieStore.CookiePolicy { get async }
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Permitting cookie storage

func setCookiePolicy(WKHTTPCookieStore.CookiePolicy, completionHandler: (() -> Void)?)

Sets a cookie policy that indicates whether the cookie store allows cookie storage.

enum CookiePolicy

An enumeration with cases that indicate whether a cookie store allows cookie storage.

