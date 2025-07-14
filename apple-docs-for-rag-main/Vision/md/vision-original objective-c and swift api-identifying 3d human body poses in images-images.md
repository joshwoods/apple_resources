

- Vision
- Original Objective-C and Swift API
-  Identifying 3D human body poses in images 

Article

# Identifying 3D human body poses in images

Detect three-dimensional human body poses using the Vision framework.

## Overview

Vision allows you to take your app’s body pose detection into the third dimension. All photos — with people in them — are a 2D representation of people in a 3D world. Starting in iOS 17 and macOS 14, Vision detects human body poses and measures 17 individual joint locations in 3D space. You access a joint location using the joint name itself, or with a joint group name that returns a collection of joints. The following illustration of a 3D model identifies the 17 joint locations that Vision detects.

Images you capture in Portrait mode using Camera — or using AVFoundation — contain depth data that helps to detect distance for each pixel. If your content contains depth data, Vision fetches it automatically. With Vision, you can build an app that tracks a person performing an exercise in 3D space, follows the arm movement during a golf swing, or captures character animations for a video game.

For more information about recognizing a body pose in 2D, see Detecting Human Body Poses in Images.

### Perform a body pose request

Detecting the position of the joints on a human body in 3D space begins with VNDetectHumanBodyPose3DRequest. The request only supports the detection and results for the most prominent person in the frame, so it generates a single observation. For example, performing a request on an image with three people — with one person being closer to the camera — returns an observation that detects the person closest to the camera.

The observation contains a collection of 17 VNHumanBodyRecognizedPoint3D objects that contain the 3D position of a joint you specify, and the parent joint it connects to. The framework doesn’t return a partial list of joints, so you get all 17 joints or none.

The request doesn’t require images with depth data to run. However, providing depth data improves detection accuracy.

```
import Vision

// Get an image from the project bundle. 
guard let filePath = Bundle.main.path(forResource: "bodypose", ofType: "heic") else { 
    return 
} 
let fileUrl = URL(fileURLWithPath: filePath) 

// Create an object to process the request.  
let requestHandler = VNImageRequestHandler(url: fileUrl) 

// Create a request to detect a body pose in 3D space. 
let request = VNDetectHumanBodyPose3DRequest() 

do {    
    // Perform the body pose request.    
    try requestHandler.perform([request])    

    // Get the observation.    
    if let observation = request.results?.first {        
        // Handle the observation.    
    }
} catch {
    print("Unable to perform the request: \(error).") 
}
```

### Handle the resulting observation

A VNHumanBodyPose3DObservation provides body pose information in 3D space, in meters. The framework normalizes 2D points — from other framework requests — to a lower-left origin. Points that a 3D body pose request returns are relative to the scene in the real world, with an origin at the root joint, located between the leftHip and rightHip.

To get a list of the available joint names, call supportedJointNames. Joints are also grouped by their location on the body. For example, the left arm group provides the left shoulder, elbow and wrist joints. To get a list of the group names, call supportedJointsGroupNames.

```
// Get a recognized joint by using a joint name. 
let leftShoulder = try observation.recognizedPoint(.leftShoulder) 
let leftElbow = try observation.recognizedPoint(.leftElbow) 
let leftWrist = try observation.recognizedPoint(.leftWrist) 

// Get a collection of joints by using a joint group name. 
let leftArm = try observation.recognizedPoints(.leftArm)
```

If there’s enough depth metadata, bodyHeight provides an estimated height of the subject, in meters; otherwise, bodyHeight returns a reference height of `1.8` meters. The framework provides a measured height only when configuring an AVCaptureSession to use the LiDAR camera. For more information about configuring your session, see Capturing depth using the LiDAR camera.

Use cameraRelativePosition(_:) to get an estimate of how far the person was away from a camera. To get an accurate understanding of where the camera was when capturing the image, use cameraOriginMatrix.

### Work with positions in 3D space

The Vision frameworks represents a 3D position as a simd_float4x4 matrix. A VNHumanBodyRecognizedPoint3D object contains the position of the joint, in meters, along with an identifier that corresponds to the joint name. It also contains the localPosition of the joint, which describes the position relative to a parentJoint.

Important

A joint’s position is always relative to the root joint.

Use pointInImage(_:) to project a 3D joint coordinate back to a 2D input image for the body joint you specify. For instance, if you want to align the 3D body pose with the 2D input image, use pointInImage(_:) to get the root joint position in the input image.

A localPosition is useful if your app is only working with one area of the body, and simplifies determining the angle between a child and parent joint.

```
import simd 

var angleVector: simd_float3 = simd_float3() 

// Get the position relative to the parent shoulder joint. 
let childPosition = leftElbow.localPosition 
let translationChild = simd_make_float3(childPosition.columns.3[0], 
                                        childPosition.columns.3[1], 
                                        childPosition.columns.3[2]) 

// The rotation around the x-axis. 
let pitch = (Float.pi / 2) 

// The rotation around the y-axis. 
let yaw = acos(translationChild.z / simd_length(translationChild)) 

// The rotation around the z-axis. 
let roll = atan2((translationChild.y), (translationChild.x)) 

// The angle between the elbow and shoulder joint. 
angleVector = simd_float3(pitch, yaw, roll)
```

For more information about matrices, see Working with Matrices.

### Use depth data as input

Depth data contains the information the system needs to reconstruct a 3D scene, and includes camera calibration data. AVDepthData serves as the container class for interfacing with depth metadata. Starting in iOS 17 and macOS 14, provide depth data when you initialize a VNImageRequestHandler with sample or pixel buffers.

Images you capture using Photo mode in Camera store depth as disparity maps — a 2D map reduced from 3D space — with calibration data. You can also configure your AVCaptureSession to use LiDAR to get depth data. For more information about working with depth, see Capturing Photos with Depth and Enhancing Live Video by Leveraging TrueDepth Camera Data.

## See Also

### 3D body pose detection

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

