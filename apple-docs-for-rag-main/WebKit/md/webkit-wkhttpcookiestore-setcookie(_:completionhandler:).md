

- WebKit
- WKHTTPCookieStore
-  setCookie(\_:completionHandler:) 

Instance Method

# setCookie(\_:completionHandler:)

Adds a cookie to the cookie store.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func setCookie(
    _ cookie: HTTPCookie,
    completionHandler: (@MainActor () -> Void)? = nil
)
```

``` source
@MainActor
func setCookie(_ cookie: HTTPCookie) async
```

## Parameters 

`cookie`  

The cookie to add.

`completionHandler`  

A completion handler block to execute asynchronously after the method successfully stores the cookie. This block has no return value and no parameters.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setCookie(_ cookie: HTTPCookie) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Managing cookies

func getAllCookies(([HTTPCookie]) -> Void)

Fetches all stored cookies asynchronously and delivers them to the specified completion handler.

func delete(HTTPCookie, completionHandler: (() -> Void)?)

Deletes the specified cookie.

