

- Foundation
- HTTPCookieStorage
-  getCookiesFor(\_:completionHandler:) 

Instance Method

# getCookiesFor(\_:completionHandler:)

Fetches cookies relevant to the specified task and passes them to the completion handler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getCookiesFor(
    _ task: URLSessionTask,
    completionHandler: @escaping ([HTTPCookie]?) -> Void
)
```

``` source
func cookies(for task: URLSessionTask) async -> [HTTPCookie]?
```

## Parameters 

`task`  

The task performing a request. The cookie storage can use the URL and other properties of this task’s request to determine which cookies to fetch.

`completionHandler`  

A completion handler that receives an array of cookies as its argument.

## See Also

### Retrieving cookies

var cookies: [HTTPCookie]?

The cookie storage’s cookies.

func cookies(for: URL) -> [HTTPCookie]?

Returns all the cookie storage’s cookies that are sent to a specified URL.

func sortedCookies(using: [NSSortDescriptor]) -> [HTTPCookie]

Returns all of the cookie storage’s cookies, sorted according to a given set of sort descriptors.

