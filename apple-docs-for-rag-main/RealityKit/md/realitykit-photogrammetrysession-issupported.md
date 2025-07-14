

- RealityKit
- PhotogrammetrySession
-  isSupported 

Type Property

# isSupported

Returns `true` if the current hardware supports Object Capture.

iOS 17.0+iPadOS 17.0+Mac Catalyst 16.0+macOS 13.0+

``` source
static var isSupported: Bool { get }
```

## See Also

### Creating the session

convenience init(input: URL, configuration: PhotogrammetrySession.Configuration) throws

Creates a session from a specified directory of images.

convenience init&lt;S>(input: S, configuration: PhotogrammetrySession.Configuration) throws

Creates a session from a sequence of samples.

