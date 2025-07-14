

- AVFoundation
- Media reading and writing
-  Caption Authoring 

API Collection

# Caption Authoring

Create captions and subtitles in industry-standard formats.

## Topics

### Captions

class AVCaption

An object that represents text to present over a time range.

class AVMutableCaption

A mutable caption subclass that you use to create new captions.

### Regions

class AVCaptionRegion

An object that represents the region in which the system presents a caption.

class AVMutableCaptionRegion

A mutable caption region subclass that you use to create new caption regions.

### Groups

class AVCaptionGroup

An object that represents zero or more captions that intersect in time.

class AVCaptionGrouper

An object that analyzes the temporal overlaps of caption objects to create caption groups for each span of concurrent captions.

### Presentation

class AVCaptionRenderer

An object that renders captions for display at a particular time.

### Reading and Writing

class AVAssetReaderOutputCaptionAdaptor

An object that reads caption group objects from an asset track that contains timed text.

class AVAssetWriterInputCaptionAdaptor

An object that appends captions to an asset writer input.

### Conversion and Validation

struct AVCaptionSettingsKey

A structure that defines dictionary keys to configure the caption converter and validator.

class AVCaptionFormatConformer

An object that converts a canonical caption to a specific format.

class AVCaptionConversionValidator

An object that validates captions for a conversion operation.

