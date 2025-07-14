

- AVFoundation
- Additional data capture
-  Metadata Types 

API Collection

# Metadata Types

Inspect the supported metadata object types that the framework supports.

## Topics

### 2D and 3D Codes

class AVMetadataMachineReadableCodeObject

Barcode information detected by a metadata capture output.

### Faces

class AVMetadataFaceObject

Face information detected by a metadata capture output.

### Bodies

class AVMetadataBodyObject

An abstract class that defines the interface for a metadata body object.

class AVMetadataCatBodyObject

An object representing a single detected cat body in a picture.

class AVMetadataDogBodyObject

An object representing a single detected dog body in a picture.

class AVMetadataHumanBodyObject

An object representing a single detected human body in a picture.

class AVMetadataHumanFullBodyObject

An object that represents a detected human full body in a picture.

### Saliency

class AVMetadataSalientObject

An object representing a single salient area in a picture.

## See Also

### Metadata capture

class AVCaptureMetadataInput

A capture input for providing timed metadata to a capture session.

class AVCaptureMetadataOutput

A capture output for processing timed metadata produced by a capture session.

class AVMetadataObject

The abstract superclass for objects provided by a metadata capture output.

