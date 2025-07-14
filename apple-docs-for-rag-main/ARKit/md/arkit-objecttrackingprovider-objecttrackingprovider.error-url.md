

- ARKit
- ObjectTrackingProvider
- ObjectTrackingProvider.Error
-  url 

Instance Property

# url

The URL for the model that failed to load, if the source was a URL.

visionOS 2.0+

``` source
let url: URL?
```

## See Also

### Inspecting an error

let bundle: Bundle?

The bundle for the model that failed to load, if the source was a bundle.

let name: String?

The name of the model that failed to load, if the source was a bundle.

var recoverySuggestion: String?

A localized message that describes how to recover from the failure.

