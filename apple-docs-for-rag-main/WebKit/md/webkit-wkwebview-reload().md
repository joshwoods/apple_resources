

- WebKit
- WKWebView
-  reload() 

Instance Method

# reload()

Reloads the current webpage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func reload() -> WKNavigation?
```

## Return Value

A new navigation object to represent the reload operation.

## See Also

### Managing the loading process

func reload(Any?)

Reloads the current webpage.

func reloadFromOrigin() -> WKNavigation?

Reloads the current webpage, and performs end-to-end revalidation of the content using cache-validating conditionals, if possible.

func reloadFromOrigin(Any?)

Reloads the current webpage, and performs end-to-end revalidation of the content using cache-validating conditionals, if possible.

func stopLoading()

Stops loading all resources on the current page.

func stopLoading(Any?)

Stops loading all resources on the current page.

