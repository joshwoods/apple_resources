

- WebKit
- WebView
-  stopLoading(\_:) 

Instance Method

# stopLoading(\_:)

An action method that stops the loading of any web frame content managed by the receiver.

macOS

``` source
@IBAction @MainActor
func stopLoading(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

Stops any content in the process of being loaded by the main frame or any of its children frames. Does nothing if no content is being loaded.

## See Also

### Loading Content

func takeStringURLFrom(Any?)

Sets the receiver’s current location by obtaining a URL string from the sender.

func reload(Any?)

An action method that reloads the current page.

func reloadFromOrigin(Any?)

Action method that performs an end-to-end revalidation using cache-validating conditionals if possible.

var estimatedProgress: Double

An estimate, as a percentage, of the amount of content that is currently loaded.

Deprecated

