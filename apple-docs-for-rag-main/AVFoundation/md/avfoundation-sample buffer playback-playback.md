

- AVFoundation
-  Sample buffer playback 

API Collection

# Sample buffer playback

Create custom controllers to play and synchronize the timing of sample buffer streams.

## Topics

### Sample buffer generation

Playing custom audio with your own player

Construct an audio player to play your custom audio data, and optionally take advantage of the advanced features of AirPlay 2.

class AVSampleBufferRequest

An object that describes a sample buffer creation request.

class AVSampleBufferGenerator

An object that creates sample buffers.

class AVSampleBufferGeneratorBatch

An object that generates sample buffers in a batch.

### Presentation

protocol AVQueuedSampleBufferRendering

Methods you can implement to enqueue sample buffers for presentation.

class AVSampleBufferRenderSynchronizer

An object used to synchronize multiple queued sample buffers to a single timeline.

class AVSampleBufferDisplayLayer

An object that displays compressed or uncompressed video frames.

class AVSampleBufferVideoRenderer

An object that enqueues video sample buffers for rendering.

class AVSampleBufferAudioRenderer

An object used to decompress audio and play compressed or uncompressed audio.

## See Also

### Playback

Media playback

Manage the playback of media assets and interstitial content, independent of how you present that content in your interface.

Offline playback and storage

Download streamed content to disk to allow offline playback, and define policies to automatically remove downloaded assets.

Streaming and AirPlay

Stream content wirelessly to other devices using AirPlay, and handle requests involving FairPlay-protected assets.

