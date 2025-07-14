

- AVFoundation
-  Video effects 

API Collection

# Video effects

Define standard video transition effects, synchronize layer animations with media timing, and create custom video compositors.

## Topics

### Core Animation integration

class AVVideoCompositionCoreAnimationTool

An object used to incorporate Core Animation into a video composition.

### Built-in video compositing

Editing and Playing HDR Video

Support high-dynamic-range (HDR) video content in your app by using the HDR editing and playback capabilities of AVFoundation.

Debugging AVFoundation audio mixes, compositions, and video compositions

Resolve common problems when creating compositions, video compositions, and audio mixes.

class AVVideoComposition

An object that describes how to compose video frames at particular points in time.

class AVMutableVideoComposition

A mutable video composition subclass.

class AVVideoCompositionInstruction

An operation that a compositor performs.

class AVMutableVideoCompositionInstruction

A mutable video composition instruction subclass.

class AVVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a composition.

class AVMutableVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a mutable composition.

### Custom video compositing

protocol AVVideoCompositing

A protocol that defines the methods custom video compositors must implement.

## See Also

### Editing

Composite assets

Combine tracks and segments of tracks from multiple assets into a composite asset that you can play or process.

QuickTime movies

Access the contents of a QuickTime movie file, and perform sample-level edits of its media tracks.

Audio mixing

Define how to mix the audio levels from multiple audio tracks over an asset’s duration.

