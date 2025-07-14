

- WebKit
- WKHTTPCookieStore
-  setCookiePolicy(\_:completionHandler:) 

Instance Method

# setCookiePolicy(\_:completionHandler:)

Sets a cookie policy that indicates whether the cookie store allows cookie storage.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
func setCookiePolicy(
    _ policy: WKHTTPCookieStore.CookiePolicy,
    completionHandler: (@MainActor () -> Void)? = nil
)
```

``` source
@MainActor
func setCookiePolicy(_ policy: WKHTTPCookieStore.CookiePolicy) async
```

## Parameters 

`policy`  

A cookie policy that indicates whether the cookie store allows cookie storage.

`completionHandler`  

A block the system invokes after it sets the cookie policy.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setCookiePolicy(_ policy: WKHTTPCookieStore.CookiePolicy) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Permitting cookie storage

func getCookiePolicy((WKHTTPCookieStore.CookiePolicy) -> Void)

Returns a cookie policy that indicates whether the cookie store allows cookie storage.

enum CookiePolicy

An enumeration with cases that indicate whether a cookie store allows cookie storage.

