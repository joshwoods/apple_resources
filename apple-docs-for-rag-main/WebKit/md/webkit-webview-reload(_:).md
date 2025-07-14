

- WebKit
- WebView
-  reload(\_:) 

Instance Method

# reload(\_:)

An action method that reloads the current page.

macOS

``` source
@IBAction @MainActor
func reload(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## See Also

### Related Documentation

var resourceLoadDelegate: (any WebResourceLoadDelegate)!

The receiver’s resource load delegate.

Deprecated

### Loading Content

func stopLoading(Any?)

An action method that stops the loading of any web frame content managed by the receiver.

func takeStringURLFrom(Any?)

Sets the receiver’s current location by obtaining a URL string from the sender.

func reloadFromOrigin(Any?)

Action method that performs an end-to-end revalidation using cache-validating conditionals if possible.

var estimatedProgress: Double

An estimate, as a percentage, of the amount of content that is currently loaded.

Deprecated

