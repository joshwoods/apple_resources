

- Vision
-  Original Objective-C and Swift API 

API Collection

# Original Objective-C and Swift API

## Topics

### Essentials

Building a feature-rich app for sports analysis

Detect and classify human activity in real time using computer vision and machine learning.

### Still-image analysis

Detecting Objects in Still Images

Locate and demarcate rectangles, faces, barcodes, and text in images using the Vision framework.

Classifying images for categorization and search

Analyze and label images using a Vision classification request.

Analyzing Image Similarity with Feature Print

Generate a feature print to compute distance between images.

class VNRequest

The abstract superclass for analysis requests.

class VNImageBasedRequest

The abstract superclass for image-analysis requests that focus on a specific part of an image.

class VNClassifyImageRequest

A request to classify an image.

class VNGenerateImageFeaturePrintRequest

An image-based request to generate feature prints from an image.

class VNFeaturePrintObservation

An observation that provides the recognized feature print.

class VNImageRequestHandler

An object that processes one or more image-analysis request pertaining to a single image.

class VNObservation

The abstract superclass for analysis results.

### Image sequence analysis

Applying Matte Effects to People in Images and Video

Generate image masks for people automatically by using semantic person-segmentation.

Detecting Human Actions in a Live Video Feed

Identify body movements by sending a person’s pose data from a series of video frames to an action-classification model.

Segmenting and colorizing individuals from a surrounding scene

Use the Vision framework to isolate and apply colors to people in an image.

class VNStatefulRequest

An abstract request type that builds evidence of a condition over time.

class VNGeneratePersonSegmentationRequest

An object that produces a matte image for a person it finds in the input image.

class VNGeneratePersonInstanceMaskRequest

An object that produces a mask of individual people it finds in the input image.

class VNDetectDocumentSegmentationRequest

An object that detects rectangular regions that contain text in the input image.

class VNSequenceRequestHandler

An object that processes image-analysis requests for each frame in a sequence.

### Image aesthetics analysis

class VNCalculateImageAestheticsScoresRequest

An object that analyzes an image for aesthetically pleasing attributes.

### Saliency analysis

Cropping Images Using Saliency

Isolate regions in an image that are most likely to draw people’s attention.

Highlighting Areas of Interest in an Image Using Saliency

Quantify and visualize where people are likely to look in an image.

class VNGenerateAttentionBasedSaliencyImageRequest

An object that produces a heat map that identifies the parts of an image most likely to draw attention.

class VNGenerateObjectnessBasedSaliencyImageRequest

A request that generates a heat map that identifies the parts of an image most likely to represent objects.

class VNSaliencyImageObservation

An observation that contains a grayscale heat map of important areas across an image.

### Object tracking

Tracking the User’s Face in Real Time

Detect and track faces from the selfie cam feed in real time.

Tracking Multiple Objects or Rectangles in Video

Apply Vision algorithms to track objects or rectangles throughout a video.

class VNTrackingRequest

The abstract superclass for image-analysis requests that track unique features across multiple images or video frames.

class VNTrackRectangleRequest

An image-analysis request that tracks movement of a previously identified rectangular object across multiple images or video frames.

class VNTrackObjectRequest

An image-analysis request that tracks the movement of a previously identified object across multiple images or video frames.

class VNDetectedObjectObservation

An observation that provides the position and extent of an image feature that an image- analysis request detects.

### Rectangle detection

class VNDetectRectanglesRequest

An image-analysis request that finds projected rectangular regions in an image.

### Face and body detection

Selecting a selfie based on capture quality

Compare face-capture quality in a set of images by using Vision.

class VNDetectFaceCaptureQualityRequest

A request that produces a floating-point number that represents the capture quality of a face in a photo.

class VNDetectFaceLandmarksRequest

An image-analysis request that finds facial features like eyes and mouth in an image.

class VNDetectFaceRectanglesRequest

A request that finds faces within an image.

class VNDetectHumanRectanglesRequest

A request that finds rectangular regions that contain people in an image.

class VNHumanObservation

An object that represents a person that the request detects.

### Body and hand pose detection

Detecting Human Body Poses in Images

Add the capability to detect human body poses to your app using the Vision framework.

Detecting Hand Poses with Vision

Create a virtual drawing app by using Vision’s capability to detect hand poses.

class VNDetectHumanBodyPoseRequest

A request that detects a human body pose.

class VNDetectHumanHandPoseRequest

A request that detects a human hand pose.

class VNRecognizedPointsObservation

An observation that provides the points the analysis recognized.

class VNHumanBodyPoseObservation

An observation that provides the body points the analysis recognized.

class VNHumanHandPoseObservation

An observation that provides the hand points the analysis recognized.

class VNPoint

An immutable object that represents a single 2D point in an image.

class VNDetectedPoint

An object that represents a normalized point in an image, along with a confidence value.

class VNRecognizedPoint

An object that represents a normalized point in an image, along with an identifier label and a confidence value.

struct VNRecognizedPointKey

The data type for all recognized point keys.

struct VNRecognizedPointGroupKey

The data type for all recognized-point group keys.

### 3D body pose detection

Identifying 3D human body poses in images

Detect three-dimensional human body poses using the Vision framework.

Detecting human body poses in 3D with Vision

Render skeletons of 3D body pose points in a scene overlaying the input image.

class VNDetectHumanBodyPose3DRequest

A request that detects points on human bodies in 3D space, relative to the camera.

class VNHumanBodyPose3DObservation

An observation that provides the 3D body points the request recognizes.

class VNRecognizedPoints3DObservation

An observation that provides the 3D points for a request.

class VNHumanBodyRecognizedPoint3D

A recognized 3D point that includes a parent joint.

class VNPoint3D

An object that represents a 3D point in an image.

class VNRecognizedPoint3D

A 3D point that includes an identifier to the point.

struct JointName

The joint names for a 3D body pose.

struct JointsGroupName

The joint group names for a 3D body pose.

### Animal detection

class VNRecognizeAnimalsRequest

A request that recognizes animals in an image.

### Animal body pose detection

Detecting animal body poses with Vision

Draw the skeleton of an animal by using Vision’s capability to detect animal body poses.

class VNDetectAnimalBodyPoseRequest

A request that detects an animal body pose.

class VNAnimalBodyPoseObservation

An observation that provides the animal body points the analysis recognizes.

### Trajectory detection

Identifying Trajectories in Video

Gain new insights into your video data by using Vision to detect trajectories.

Detecting moving objects in a video

Identify the trajectory of a thrown object by using Vision.

class VNDetectTrajectoriesRequest

A request that detects the trajectories of shapes moving along a parabolic path.

### Contour detection

class VNDetectContoursRequest

A request that detects the contours of the edges of an image.

### Optical flow

class VNGenerateOpticalFlowRequest

An object that generates directional change vectors for each pixel in the targeted image.

class VNTrackOpticalFlowRequest

An object that determines the direction change of vectors for each pixel from a previous to current image.

### Barcode detection

class VNDetectBarcodesRequest

A request that detects barcodes in an image.

enum VNBarcodeCompositeType

Composite types for barcode requests.

### Text detection

class VNDetectTextRectanglesRequest

An image-analysis request that finds regions of visible text in an image.

class VNTextObservation

Information about regions of text that an image-analysis request detects.

### Text recognition

Recognizing Text in Images

Add text-recognition features to your app using the Vision framework.

Structuring Recognized Text on a Document

Detect, recognize, and structure text on a business card or receipt using Vision and VisionKit.

Extracting phone numbers from text in images

Analyze and filter phone numbers from text in live capture by using Vision.

Locating and displaying recognized text

Perform text recognition on a photo using the Vision framework’s text-recognition request.

class VNRecognizeTextRequest

An image-analysis request that finds and recognizes text in an image.

class VNRecognizedTextObservation

A request that detects and recognizes regions of text in an image.

### Object recognition

Recognizing Objects in Live Capture

Apply Vision algorithms to identify objects in real-time video.

Understanding a Dice Roll with Vision and Object Detection

Detect dice position and values shown in a camera frame, and determine the end of a roll by leveraging a dice detection model.

class VNRecognizedObjectObservation

A detected object observation with an array of classification labels that classify the recognized object.

### Request progress tracking

protocol VNRequestProgressProviding

A protocol for providing progress information on long-running tasks in Vision.

typealias VNRequestProgressHandler

A block executed at intervals during the processing of a Vision request.

### Horizon detection

class VNDetectHorizonRequest

An image-analysis request that determines the horizon angle in an image.

class VNHorizonObservation

The horizon angle information that an image-analysis request detects.

### Image alignment

Aligning Similar Images

Construct a composite image from images that capture the same scene.

class VNTargetedImageRequest

The abstract superclass for image analysis requests that operate on both the processed image and a secondary image.

class VNImageRegistrationRequest

The abstract superclass for image-analysis requests that align images according to their content.

class VNTranslationalImageRegistrationRequest

An image-analysis request that determines the affine transform necessary to align the content of two images.

class VNTrackTranslationalImageRegistrationRequest

An image-analysis request, as a stateful request you track over time, that determines the affine transform necessary to align the content of two images.

class VNHomographicImageRegistrationRequest

An image-analysis request that determines the perspective warp matrix necessary to align the content of two images.

class VNTrackHomographicImageRegistrationRequest

An image-analysis request, as a stateful request you track over time, that determines the perspective warp matrix necessary to align the content of two images.

class VNImageAlignmentObservation

The abstract superclass for image-analysis results that describe the relative alignment of two images.

class VNImageTranslationAlignmentObservation

Affine transform information that an image-alignment request produces.

class VNImageHomographicAlignmentObservation

An object that represents a perspective warp transformation.

### Image background removal

Applying visual effects to foreground subjects

Segment the foreground subjects of an image and composite them to a new background with visual effects.

class VNInstanceMaskObservation

An observation that contains an instance mask that labels instances in the mask.

class VNGenerateForegroundInstanceMaskRequest

A request that generates an instance mask of noticable objects to separate from the background.

let VNGenerateForegroundInstanceMaskRequestRevision1: Int

A constant for specifying the first revision of the foreground instance mask request.

### Machine learning image analysis

Classifying Images with Vision and Core ML

Crop and scale photos using the Vision framework and classify them with a Core ML model.

Training a Create ML Model to Classify Flowers

Train a flower classifier using Create ML in Swift Playgrounds, and apply the resulting model to real-time image classification using Vision.

class VNCoreMLRequest

An image-analysis request that uses a Core ML model to process images.

class VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

class VNPixelBufferObservation

An object that represents an image that an image-analysis request produces.

class VNCoreMLFeatureValueObservation

An object that represents a collection of key-value information that a Core ML image-analysis request produces.

### Coordinate conversion

func VNImagePointForNormalizedPoint(CGPoint, Int, Int) -> CGPoint

Projects a point in normalized coordinates into image coordinates.

func VNNormalizedPointForImagePoint(CGPoint, Int, Int) -> CGPoint

Projects a point from image coordinates into normalized coordinates.

func VNImagePointForNormalizedPointUsingRegionOfInterest(CGPoint, Int, Int, CGRect) -> CGPoint

Projects a point from a region of interest within the normalized coordinates into image coordinates.

func VNNormalizedPointForImagePointUsingRegionOfInterest(CGPoint, Int, Int, CGRect) -> CGPoint

Projects a point from a region of interest within the image coordinates into normalized coordinates.

func VNImageRectForNormalizedRect(CGRect, Int, Int) -> CGRect

Projects a rectangle from normalized coordinates into image coordinates.

func VNNormalizedRectForImageRect(CGRect, Int, Int) -> CGRect

Projects a rectangle from image coordinates into normalized coordinates.

func VNImageRectForNormalizedRectUsingRegionOfInterest(CGRect, Int, Int, CGRect) -> CGRect

Projects a rectangle from a region of interest within the normalized coordinates into image coordinates.

func VNNormalizedRectForImageRectUsingRegionOfInterest(CGRect, Int, Int, CGRect) -> CGRect

Projects a rectangle from a region of interest within the image coordinates space into normalized coordinates.

let VNNormalizedIdentityRect: CGRect

A normalized identity rectangle with an origin of zero and unit length and width.

func VNNormalizedRectIsIdentityRect(CGRect) -> Bool

Returns a Boolean value that indicates whether the rectangle has an origin of zero and unit length and width.

func VNImagePointForFaceLandmarkPoint(vector_float2, CGRect, Int, Int) -> CGPoint

Returns the image coordinates of a specified face landmark point.

func VNNormalizedFaceBoundingBoxPointForLandmarkPoint(vector_float2, CGRect, Int, Int) -> CGPoint

Returns the coordinates of a specified face landmark point, in bounding box coordinates.

### Utilities

struct VNComputeStage

Types that represent the compute stage.

class VNGeometryUtils

Utility methods to determine the geometries of various Vision types.

class VNVideoProcessor

An object that performs offline analysis of video content.

### Common data types

class VNCircle

An immutable 2D circle represented by its center point and radius.

class VNVector

An immutable 2D vector represented by its x-axis and y-axis projections.

### Errors

let VNErrorDomain: String

The domain of errors that the framework generates.

enum VNErrorCode

Constants that identify errors from the framework.

### Version and revision numbers

var VNVisionVersionNumber: Double

The current version number of the Vision framework.

let VNDetectAnimalBodyPoseRequestRevision1: Int

A value that indicates the first revision for an animal body-pose request.

let VNDetectHumanBodyPose3DRequestRevision1: Int

A value that indicates the first revision for a human 3D body pose request.

let VNTrackHomographicImageRegistrationRequestRevision1: Int

A value that indicates the first revision for a homographic image-registration request.

let VNTrackTranslationalImageRegistrationRequestRevision1: Int

A value that indicates the first revision for a translational image-registration request.

let VNTrackOpticalFlowRequestRevision1: Int

A value that indicates the first revision for an optial-flow request.

let VNClassifyImageRequestRevision1: Int

A constant for specifying the first revision of the image-classification request.

let VNClassifyImageRequestRevision2: Int

A value that indicates the second revision for an image-classification request.

let VNGenerateObjectnessBasedSaliencyImageRequestRevision2: Int

A value that indicates the second revision for an image-classification request.

let VNGenerateAttentionBasedSaliencyImageRequestRevision2: Int

A value that indicates the second revision for an attention-saliency image request.

let VNGenerateImageFeaturePrintRequestRevision1: Int

A constant for specifying the first revision of the feature-print request.

let VNGenerateImageFeaturePrintRequestRevision2: Int

A value that indicates the second revision for a feature-print request.

let VNDetectFaceCaptureQualityRequestRevision3: Int

A value that indicates the third revision for a face capture-quality request.

let VNDetectBarcodesRequestRevision4: Int

A value that indicates the fourth revision for a barcode request.

let VNCalculateImageAestheticsScoresRequestRevision1: Int

A value that indicates the first revision for an aesthetics scores request.

let VNRequestRevisionUnspecified: Int

A constant for specifying an unspecified request revision.

### Macros

Macros

