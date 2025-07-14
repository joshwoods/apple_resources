

- Foundation
- HTTPCookieStorage
-  sortedCookies(using:) 

Instance Method

# sortedCookies(using:)

Returns all of the cookie storage’s cookies, sorted according to a given set of sort descriptors.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sortedCookies(using sortOrder: [NSSortDescriptor]) -> [HTTPCookie]
```

## Parameters 

`sortOrder`  

The sort descriptors to use for sorting, as an array of NSSortDescriptor objects.

## Return Value

The cookie storage’s cookies, sorted according to `sortOrder`, as an array of HTTPCookie objects.

## See Also

### Retrieving cookies

var cookies: [HTTPCookie]?

The cookie storage’s cookies.

func getCookiesFor(URLSessionTask, completionHandler: ([HTTPCookie]?) -> Void)

Fetches cookies relevant to the specified task and passes them to the completion handler.

func cookies(for: URL) -> [HTTPCookie]?

Returns all the cookie storage’s cookies that are sent to a specified URL.

