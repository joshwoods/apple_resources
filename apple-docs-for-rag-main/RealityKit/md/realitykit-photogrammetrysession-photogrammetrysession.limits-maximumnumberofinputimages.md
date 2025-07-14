

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Limits
-  maximumNumberOfInputImages 

Instance Property

# maximumNumberOfInputImages

Returns the maximum number of input images or samples that the session can use for reconstruction. If more than this number are provided, any in excess of the limit will be ignored and an `.invalidSample` message for the sample will be output.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
var maximumNumberOfInputImages: Int { get }
```

