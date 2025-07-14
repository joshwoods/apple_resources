

- ARKit
- ARKit in iOS
-  Data Management 

API Collection

# Data Management

Obtain detailed information about skeletal and face geometry, and saved world data.

## Topics

### Body Data

Capturing Body Motion in 3D

Track a person in the physical environment and visualize their motion by applying the same body movements to a virtual character.

class ARBody2D

The screen-space representation of a person ARKit recognizes in the camera feed.

class ARSkeleton3D

The skeleton of a human body that ARKit tracks in 3D space.

class ARSkeleton2D

An object that describes the locations of a body’s joints in the camera feed.

class ARSkeleton

The interface for the skeleton of a tracked body.

class ARSkeletonDefinition

The hierarchy of joints and their names.

### Face Data

Tracking and visualizing faces

Detect faces in a front-camera AR experience, overlay virtual content, and animate facial expressions in real-time.

Combining user face-tracking and world tracking

Track the user’s face in an app that displays an AR experience with the rear camera.

class ARFaceGeometry

A 3D mesh describing face topology for use in face-tracking AR sessions.

class ARSCNFaceGeometry

A SceneKit representation of face topology for use with face information that an AR session provides.

### World Data

Saving and loading world data

Serialize a world-tracking session to resume it later on.

class ARWorldMap

The state in a world-tracking AR session during which a device maps the user’s position in physical space and proximity to anchor objects.

## See Also

### Virtual Content

Content Anchors

Identify items in the physical environment, including planar surfaces, images, physical objects, body positions, and faces.

Environmental Analysis

Analyze the video from the cameras and the accompanying data, and use ray-casting and depth-map information to determine the location of items.

Camera, Lighting, and Effects

Determine the camera position and lighting for the current session, and apply effects, such as occlusion, to elements of the environment.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

