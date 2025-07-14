

- WebKit
- WKHTTPCookieStore
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes an observer from the cookie store.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func remove(_ observer: any WKHTTPCookieStoreObserver)
```

## Parameters 

`observer`  

The observer object to remove.

## See Also

### Observing cookie store changes

func add(any WKHTTPCookieStoreObserver)

Adds an observer to the cookie store.

protocol WKHTTPCookieStoreObserver

The methods to adopt in an object that monitors changes to a webpage’s cookies.

