

- AVFoundation
- AVVideoCompositionInstructionProtocol
-  passthroughTrackID 

Instance Property

# passthroughTrackID

An identifier of a source track to pass through without compositing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var passthroughTrackID: CMPersistentTrackID { get }
```

**Required**

## Discussion

If an instruction indicates to pass through a source frame without compositing, this property returns the corresponding track identifier. The compositor isn’t run for the duration of the instruction, and instead passes the source frame through to the output. The system automatically matches the required dimensions, clean aperture, and pixel aspect ratio values of the source buffer.

## See Also

### Getting Track ID Settings

var requiredSourceTrackIDs: [NSValue]?

The identifiers of the video tracks the instruction requires to compose frames.

**Required**

var requiredSourceSampleDataTrackIDs: [NSNumber]

The identifiers of the sample data tracks the instruction requires to compose frames.

