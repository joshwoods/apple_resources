

- ARKit
- ARKit in iOS
-  Content Anchors 

API Collection

# Content Anchors

Identify items in the physical environment, including planar surfaces, images, physical objects, body positions, and faces.

## Overview

Anchors identify the position of items in your augmented reality session. Use anchors to obtain information about the item itself, or about the thing it represents. For example, use an ARPlaneAnchor to determine the location of a planar surface.

## Topics

### Surface Detection

Tracking and visualizing planes

Detect surfaces in the physical environment and visualize their shape and location in 3D space.

class ARPlaneAnchor

An anchor for a 2D planar surface that ARKit detects in the physical environment.

class ARMeshAnchor

An anchor for a physical object that ARKit detects and recreates virtually using a polygonal mesh.

### Image Detection

Tracking and altering images

Create images from rectangular shapes found in the user’s environment, and augment their appearance.

Detecting Images in an AR Experience

React to known 2D images in the user’s environment, and use their positions to place AR content.

class ARImageAnchor

An anchor for a known image that ARKit detects in the physical environment.

class ARReferenceImage

A 2D image that you want ARKit to detect in the physical environment.

### Physical Objects

Visualizing and interacting with a reconstructed scene

Estimate the shape of the physical environment using a polygonal mesh.

Scanning and Detecting 3D Objects

Record spatial features of real-world objects, then use the results to find those objects in the user’s environment and trigger AR content.

class ARObjectAnchor

An anchor for a real-world 3D object that ARKit detects in the physical environment.

class ARReferenceObject

The description of a 3D object that you want ARKit to detect in the physical environment.

### Body Position Tracking

Capturing Body Motion in 3D

Track a person in the physical environment and visualize their motion by applying the same body movements to a virtual character.

Rigging a Model for Motion Capture

Configure custom 3D models so ARKit’s human body-tracking feature can control them.

Validating a Model for Motion Capture

Verify that your character model matches ARKit’s Motion Capture requirements.

class ARBodyAnchor

An anchor that tracks the position and movement of a human body in the rear-facing camera.

### Face Tracking

Tracking and visualizing faces

Detect faces in a front-camera AR experience, overlay virtual content, and animate facial expressions in real-time.

Combining user face-tracking and world tracking

Track the user’s face in an app that displays an AR experience with the rear camera.

class ARFaceAnchor

An anchor for a unique face that is visible in the front-facing camera.

### Geotracking

Tracking geographic locations in AR

Track specific geographic areas of interest and render them in an AR experience.

class ARGeoAnchor

An anchor that identifies a geographic location using latitude, longitude, and altitude data.

### Multiuser Experiences

class ARParticipantAnchor

An anchor for another user in multiuser augmented reality experiences.

### App Clip Codes

Interacting with App Clip Codes in AR

Display content and provide services in an AR experience with App Clip Codes.

class ARAppClipCodeAnchor

An anchor that tracks the position and orientation of an App Clip Code in the physical environment.

### Text Annotations

Creating screen annotations for objects in an AR experience

Annotate an AR experience with virtual sticky notes that you display onscreen over real and virtual objects.

Recognizing and Labeling Arbitrary Objects

Create anchors that track objects you recognize in the camera feed, using a custom optical-recognition algorithm.

### Common Types

class ARAnchor

An object that specifies the position and orientation of an item in the physical environment.

protocol ARAnchorCopying

Support for custom anchor subclasses.

protocol ARTrackable

An interface for objects that track the location of real-world objects or locations.

## See Also

### Virtual Content

Environmental Analysis

Analyze the video from the cameras and the accompanying data, and use ray-casting and depth-map information to determine the location of items.

Camera, Lighting, and Effects

Determine the camera position and lighting for the current session, and apply effects, such as occlusion, to elements of the environment.

Data Management

Obtain detailed information about skeletal and face geometry, and saved world data.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

