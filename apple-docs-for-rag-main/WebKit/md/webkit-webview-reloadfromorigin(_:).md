

- WebKit
- WebView
-  reloadFromOrigin(\_:) 

Instance Method

# reloadFromOrigin(\_:)

Action method that performs an end-to-end revalidation using cache-validating conditionals if possible.

macOS

``` source
@IBAction @MainActor
func reloadFromOrigin(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## See Also

### Related Documentation

func reloadFromOrigin()

Performs an end-to-end revalidation using cache-validating conditionals if possible.

Deprecated

### Loading Content

func stopLoading(Any?)

An action method that stops the loading of any web frame content managed by the receiver.

func takeStringURLFrom(Any?)

Sets the receiver’s current location by obtaining a URL string from the sender.

func reload(Any?)

An action method that reloads the current page.

var estimatedProgress: Double

An estimate, as a percentage, of the amount of content that is currently loaded.

Deprecated

