

- Foundation
- HTTPCookieStorage
-  setCookie(\_:) 

Instance Method

# setCookie(\_:)

Stores a specified cookie in the cookie storage if the cookie accept policy permits.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setCookie(_ cookie: HTTPCookie)
```

## Parameters 

`cookie`  

The cookie to store.

## Discussion

The cookie replaces an existing cookie with the same name, domain, and path, if one exists in the cookie storage. This method accepts the cookie only if the storage’s cookie accept policy is HTTPCookie.AcceptPolicy.always or HTTPCookie.AcceptPolicy.onlyFromMainDocumentDomain. The cookie is ignored if the storage’s cookie accept policy is HTTPCookie.AcceptPolicy.never.

## See Also

### Adding and removing cookies

func removeCookies(since: Date)

Removes cookies that were stored after a given date.

func deleteCookie(HTTPCookie)

Deletes the specified cookie from the cookie storage.

func setCookies([HTTPCookie], for: URL?, mainDocumentURL: URL?)

Adds an array of cookies to the cookie storage if the storage’s cookie acceptance policy permits.

func storeCookies([HTTPCookie], for: URLSessionTask)

Stores an array of cookies in the cookie storage, on behalf of the provided task, if the cookie accept policy permits.

