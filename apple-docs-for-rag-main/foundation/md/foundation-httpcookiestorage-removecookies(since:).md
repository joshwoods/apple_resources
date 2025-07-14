

- Foundation
- HTTPCookieStorage
-  removeCookies(since:) 

Instance Method

# removeCookies(since:)

Removes cookies that were stored after a given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeCookies(since date: Date)
```

## Parameters 

`date`  

The date after which cookies should be removed.

## See Also

### Adding and removing cookies

func deleteCookie(HTTPCookie)

Deletes the specified cookie from the cookie storage.

func setCookie(HTTPCookie)

Stores a specified cookie in the cookie storage if the cookie accept policy permits.

func setCookies([HTTPCookie], for: URL?, mainDocumentURL: URL?)

Adds an array of cookies to the cookie storage if the storage’s cookie acceptance policy permits.

func storeCookies([HTTPCookie], for: URLSessionTask)

Stores an array of cookies in the cookie storage, on behalf of the provided task, if the cookie accept policy permits.

