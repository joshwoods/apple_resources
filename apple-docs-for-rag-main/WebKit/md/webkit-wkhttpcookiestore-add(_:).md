

- WebKit
- WKHTTPCookieStore
-  add(\_:) 

Instance Method

# add(\_:)

Adds an observer to the cookie store.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func add(_ observer: any WKHTTPCookieStoreObserver)
```

## Parameters 

`observer`  

The observer object to add. The cookie store doesn’t maintain a strong reference to the object you specify. You are responsible for removing your observer object before it becomes invalid.

## See Also

### Observing cookie store changes

func remove(any WKHTTPCookieStoreObserver)

Removes an observer from the cookie store.

protocol WKHTTPCookieStoreObserver

The methods to adopt in an object that monitors changes to a webpage’s cookies.

