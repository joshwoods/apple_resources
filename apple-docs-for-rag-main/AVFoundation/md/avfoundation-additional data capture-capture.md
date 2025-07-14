

- AVFoundation
-  Additional data capture 

API Collection

# Additional data capture

Capture additional data including depth and metadata, and synchronize capture from multiple outputs.

## Topics

### Depth data capture

Capturing Photos with Depth

Get a depth map with a photo to create effects like the system camera’s Portrait mode (on compatible devices).

Creating Auxiliary Depth Data Manually

Generate a depth image and attach it to your own image.

Capturing depth using the LiDAR camera

Access the LiDAR camera on supporting devices to capture precise depth data.

AVCamFilter: Applying Filters to a Capture Stream

Render a capture stream with rose-colored filtering and depth effects.

Streaming Depth Data from the TrueDepth Camera

Visualize depth data in 2D and 3D from the TrueDepth camera.

Enhancing Live Video by Leveraging TrueDepth Camera Data

Apply your own background to a live capture feed streamed from the front-facing TrueDepth camera.

class AVCaptureDepthDataOutput

A capture output that records scene depth information on compatible camera devices.

class AVDepthData

A container for per-pixel distance or disparity information captured by compatible camera devices.

class AVCameraCalibrationData

Information about the camera characteristics used to capture images and depth data.

### Metadata capture

class AVCaptureMetadataInput

A capture input for providing timed metadata to a capture session.

class AVCaptureMetadataOutput

A capture output for processing timed metadata produced by a capture session.

class AVMetadataObject

The abstract superclass for objects provided by a metadata capture output.

Metadata Types

Inspect the supported metadata object types that the framework supports.

### Synchronized capture

class AVCaptureDataOutputSynchronizer

An object that coordinates time-matched delivery of data from multiple capture outputs.

class AVCaptureSynchronizedDataCollection

A set of data samples collected simultaneously from multiple capture outputs.

class AVCaptureSynchronizedSampleBufferData

A container for video or audio samples collected using synchronized capture.

class AVCaptureSynchronizedMetadataObjectData

A container for metadata objects collected using synchronized capture.

class AVCaptureSynchronizedDepthData

A container for scene depth information collected using synchronized capture.

class AVCaptureSynchronizedData

The abstract superclass for media samples collected using synchronized capture.

## See Also

### Capture

Capture setup

Configure built-in cameras and microphones, and external capture devices, for media capture.

Photo capture

Capture high-quality still images, Live Photos, and supporting photo data.

Audio and video capture

Capture audio and video directly to media files, or capture streams of media for direct access to media sample buffers.

