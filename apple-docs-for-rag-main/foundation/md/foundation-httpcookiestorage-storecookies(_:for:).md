

- Foundation
- HTTPCookieStorage
-  storeCookies(\_:for:) 

Instance Method

# storeCookies(\_:for:)

Stores an array of cookies in the cookie storage, on behalf of the provided task, if the cookie accept policy permits.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func storeCookies(
    _ cookies: [HTTPCookie],
    for task: URLSessionTask
)
```

## Parameters 

`cookies`  

The cookies to add.

`task`  

The task that handles the response. Override this method and inspect this parameter if you need to alter your cookie storage strategy based on properties of the task.

## See Also

### Adding and removing cookies

func removeCookies(since: Date)

Removes cookies that were stored after a given date.

func deleteCookie(HTTPCookie)

Deletes the specified cookie from the cookie storage.

func setCookie(HTTPCookie)

Stores a specified cookie in the cookie storage if the cookie accept policy permits.

func setCookies([HTTPCookie], for: URL?, mainDocumentURL: URL?)

Adds an array of cookies to the cookie storage if the storage’s cookie acceptance policy permits.

