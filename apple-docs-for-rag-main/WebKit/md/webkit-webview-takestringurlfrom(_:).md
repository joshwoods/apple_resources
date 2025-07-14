

- WebKit
- WebView
-  takeStringURLFrom(\_:) 

Instance Method

# takeStringURLFrom(\_:)

Sets the receiver’s current location by obtaining a URL string from the sender.

macOS

``` source
@IBAction @MainActor
func takeStringURLFrom(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This method sets the receiver’s current location to the value obtained by sending a `stringValue` message to `sender`, then starts loading the URL returned by `sender`.

## See Also

### Related Documentation

func load(URLRequest!)

Connects to a given URL by initiating an asynchronous client request.

Deprecated

### Loading Content

func stopLoading(Any?)

An action method that stops the loading of any web frame content managed by the receiver.

func reload(Any?)

An action method that reloads the current page.

func reloadFromOrigin(Any?)

Action method that performs an end-to-end revalidation using cache-validating conditionals if possible.

var estimatedProgress: Double

An estimate, as a percentage, of the amount of content that is currently loaded.

Deprecated

