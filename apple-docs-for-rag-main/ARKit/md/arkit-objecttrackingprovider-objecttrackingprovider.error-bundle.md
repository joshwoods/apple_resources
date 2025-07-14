

- ARKit
- ObjectTrackingProvider
- ObjectTrackingProvider.Error
-  bundle 

Instance Property

# bundle

The bundle for the model that failed to load, if the source was a bundle.

visionOS 2.0+

``` source
let bundle: Bundle?
```

## See Also

### Inspecting an error

let name: String?

The name of the model that failed to load, if the source was a bundle.

var recoverySuggestion: String?

A localized message that describes how to recover from the failure.

let url: URL?

The URL for the model that failed to load, if the source was a URL.

