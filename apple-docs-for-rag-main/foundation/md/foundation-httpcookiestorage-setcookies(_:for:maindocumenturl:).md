

- Foundation
- HTTPCookieStorage
-  setCookies(\_:for:mainDocumentURL:) 

Instance Method

# setCookies(\_:for:mainDocumentURL:)

Adds an array of cookies to the cookie storage if the storage’s cookie acceptance policy permits.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setCookies(
    _ cookies: [HTTPCookie],
    for URL: URL?,
    mainDocumentURL: URL?
)
```

## Parameters 

`cookies`  

The cookies to add.

`URL`  

The URL associated with the added cookies.

`mainDocumentURL`  

The URL of the main HTML document for the top-level frame, if known. The value can be `nil`. This URL is used to determine whether the cookie should be accepted if the cookie accept policy is HTTPCookie.AcceptPolicy.onlyFromMainDocumentDomain.

## Discussion

Cookies in the array will replace existing cookies with the same name, domain, and path in the cookie storage. If the storage has an accept policy of HTTPCookie.AcceptPolicy.never, the cookies are ignored.

To store cookies from a set of response headers, an application can use cookies(withResponseHeaderFields:for:) passing a header field dictionary and then use this method to store the resulting cookies in accordance with the cookie storage’s cookie acceptance policy.

If you override this method, also override storeCookies(_:for:).

## See Also

### Adding and removing cookies

func removeCookies(since: Date)

Removes cookies that were stored after a given date.

func deleteCookie(HTTPCookie)

Deletes the specified cookie from the cookie storage.

func setCookie(HTTPCookie)

Stores a specified cookie in the cookie storage if the cookie accept policy permits.

func storeCookies([HTTPCookie], for: URLSessionTask)

Stores an array of cookies in the cookie storage, on behalf of the provided task, if the cookie accept policy permits.

