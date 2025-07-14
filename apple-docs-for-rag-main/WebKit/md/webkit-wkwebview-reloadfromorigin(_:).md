

- WebKit
- WKWebView
-  reloadFromOrigin(\_:) 

Instance Method

# reloadFromOrigin(\_:)

Reloads the current webpage, and performs end-to-end revalidation of the content using cache-validating conditionals, if possible.

macOS

``` source
@IBAction @MainActor
func reloadFromOrigin(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the message.

## Discussion

Make this method the action of any controls that trigger a reload of your web content. Connect your controls to this method programmatically or in Interface Builder.

## See Also

### Managing the loading process

func reload() -> WKNavigation?

Reloads the current webpage.

func reload(Any?)

Reloads the current webpage.

func reloadFromOrigin() -> WKNavigation?

Reloads the current webpage, and performs end-to-end revalidation of the content using cache-validating conditionals, if possible.

func stopLoading()

Stops loading all resources on the current page.

func stopLoading(Any?)

Stops loading all resources on the current page.

