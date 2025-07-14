

- ARKit
- ObjectTrackingProvider
- ObjectTrackingProvider.Error
-  recoverySuggestion 

Instance Property

# recoverySuggestion

A localized message that describes how to recover from the failure.

visionOS 2.0+

``` source
var recoverySuggestion: String? { get }
```

## See Also

### Inspecting an error

let bundle: Bundle?

The bundle for the model that failed to load, if the source was a bundle.

let name: String?

The name of the model that failed to load, if the source was a bundle.

let url: URL?

The URL for the model that failed to load, if the source was a URL.

