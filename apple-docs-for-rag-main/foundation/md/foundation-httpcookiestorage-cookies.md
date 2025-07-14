

- Foundation
- HTTPCookieStorage
-  cookies 

Instance Property

# cookies

The cookie storage’s cookies.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var cookies: [HTTPCookie]? { get }
```

## Discussion

If you want to sort the cookie storage’s cookies, you should use the sortedCookies(using:) method instead of sorting the result of this method.

## See Also

### Retrieving cookies

func getCookiesFor(URLSessionTask, completionHandler: ([HTTPCookie]?) -> Void)

Fetches cookies relevant to the specified task and passes them to the completion handler.

func cookies(for: URL) -> [HTTPCookie]?

Returns all the cookie storage’s cookies that are sent to a specified URL.

func sortedCookies(using: [NSSortDescriptor]) -> [HTTPCookie]

Returns all of the cookie storage’s cookies, sorted according to a given set of sort descriptors.

