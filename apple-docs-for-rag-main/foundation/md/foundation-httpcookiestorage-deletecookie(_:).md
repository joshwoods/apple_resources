

- Foundation
- HTTPCookieStorage
-  deleteCookie(\_:) 

Instance Method

# deleteCookie(\_:)

Deletes the specified cookie from the cookie storage.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func deleteCookie(_ cookie: HTTPCookie)
```

## Parameters 

`cookie`  

The cookie to delete.

## See Also

### Adding and removing cookies

func removeCookies(since: Date)

Removes cookies that were stored after a given date.

func setCookie(HTTPCookie)

Stores a specified cookie in the cookie storage if the cookie accept policy permits.

func setCookies([HTTPCookie], for: URL?, mainDocumentURL: URL?)

Adds an array of cookies to the cookie storage if the storage’s cookie acceptance policy permits.

func storeCookies([HTTPCookie], for: URLSessionTask)

Stores an array of cookies in the cookie storage, on behalf of the provided task, if the cookie accept policy permits.

