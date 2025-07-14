

- RealityKit
- PhotogrammetrySession
-  init(input:configuration:) 

Initializer

# init(input:configuration:)

Creates a session from a specified directory of images.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
convenience init(
    input: URL,
    configuration: PhotogrammetrySession.Configuration = Configuration()
) throws
```

## Parameters 

`input`  

The directory URL containing a folder of images to use as reconstruction inputs.

`configuration`  

The configuration to use for this session.

## Discussion

Creates a new session instance using all images in the specified URL input directory URL as samples for reconstruction.

Throws

If `input` is not a file URL.

## See Also

### Creating the session

convenience init&lt;S>(input: S, configuration: PhotogrammetrySession.Configuration) throws

Creates a session from a sequence of samples.

static var isSupported: Bool

Returns `true` if the current hardware supports Object Capture.

