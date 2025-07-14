

- ARKit
- ObjectTrackingProvider
- ObjectTrackingProvider.Error
-  name 

Instance Property

# name

The name of the model that failed to load, if the source was a bundle.

visionOS 2.0+

``` source
let name: String?
```

## See Also

### Inspecting an error

let bundle: Bundle?

The bundle for the model that failed to load, if the source was a bundle.

var recoverySuggestion: String?

A localized message that describes how to recover from the failure.

let url: URL?

The URL for the model that failed to load, if the source was a URL.

