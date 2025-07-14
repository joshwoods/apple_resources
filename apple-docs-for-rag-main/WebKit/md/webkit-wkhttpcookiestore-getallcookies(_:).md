

- WebKit
- WKHTTPCookieStore
-  getAllCookies(\_:) 

Instance Method

# getAllCookies(\_:)

Fetches all stored cookies asynchronously and delivers them to the specified completion handler.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func getAllCookies(_ completionHandler: @escaping @MainActor ([HTTPCookie]) -> Void)
```

``` source
@MainActor
func allCookies() async -> [HTTPCookie]
```

## Parameters 

`completionHandler`  

A completion handler block to execute asynchronously with the results. This block has no return value and takes the following parameter:

cookieArray  
An array of HTTPCookie objects. If the store contains no cookies, this parameter contains an empty array.

## Discussion

Use this method to get the set of cookies currently associated with your web view. Iterate over the contents of the provided array to retrieve the specific cookie you need for your code.

## See Also

### Managing cookies

func setCookie(HTTPCookie, completionHandler: (() -> Void)?)

Adds a cookie to the cookie store.

func delete(HTTPCookie, completionHandler: (() -> Void)?)

Deletes the specified cookie.

