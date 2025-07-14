

- Foundation
- HTTPCookieStorage
-  cookies(for:) 

Instance Method

# cookies(for:)

Returns all the cookie storage’s cookies that are sent to a specified URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cookies(for URL: URL) -> [HTTPCookie]?
```

## Parameters 

`URL`  

The URL to filter on.

## Return Value

An array of cookies whose URL matches the provided URL.

## Discussion

You can use the requestHeaderFields(with:) method of HTTPCookie to turn the array returned by this method into a set of header fields to add to a URLRequest object (or NSMutableURLRequest in Objective-C).

If you override this method, also override getCookiesFor(_:completionHandler:).

## See Also

### Retrieving cookies

var cookies: [HTTPCookie]?

The cookie storage’s cookies.

func getCookiesFor(URLSessionTask, completionHandler: ([HTTPCookie]?) -> Void)

Fetches cookies relevant to the specified task and passes them to the completion handler.

func sortedCookies(using: [NSSortDescriptor]) -> [HTTPCookie]

Returns all of the cookie storage’s cookies, sorted according to a given set of sort descriptors.

