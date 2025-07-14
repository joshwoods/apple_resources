

- ARKit
-  ARKit in iOS 

API Collection

# ARKit in iOS

Integrate iOS device camera and motion features to produce augmented reality experiences in your app or game.

## Topics

### Essentials

Verifying Device Support and User Permission

Check whether your app can use ARKit and respect user privacy at runtime.

USDZ schemas for AR

Add augmented reality functionality to your 3D content using USDZ schemas.

### Setup

Choosing Which Camera Feed to Augment

Add visual effects to the user’s environment in an AR experience through the front or rear camera.

Managing Session Life Cycle and Tracking Quality

Keep the user informed on the current session state and recover from interruptions.

Displaying an AR Experience with Metal

Control rendering of your app’s virtual content on top of a camera feed.

class ARSession

The object that manages the major tasks associated with every AR experience, such as motion tracking, camera passthrough, and image analysis.

Configuration Objects

Configure your augmented reality session to detect and track specific types of content.

### Views

@MainActor @objc @preconcurrency class ARView

A view that enables you to display an AR experience with RealityKit.

class ARSCNView

A view that blends virtual 3D content from SceneKit into your augmented reality experience.

class ARSKView

A view that blends virtual 2D content from SpriteKit into the 3D space of an augmented reality experience.

class ARCoachingOverlayView

A view that displays standardized onboarding instructions to direct users toward a specific goal.

### Virtual Content

Content Anchors

Identify items in the physical environment, including planar surfaces, images, physical objects, body positions, and faces.

Environmental Analysis

Analyze the video from the cameras and the accompanying data, and use ray-casting and depth-map information to determine the location of items.

Camera, Lighting, and Effects

Determine the camera position and lighting for the current session, and apply effects, such as occlusion, to elements of the environment.

Data Management

Obtain detailed information about skeletal and face geometry, and saved world data.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

### AR Quick Look

Add an AR experience to your app or website, or customize your content’s appearance in Quick Look.

Previewing a Model with AR Quick Look

Display a model or scene that the user can move, scale, and share with others.

Adding Visual Effects in AR Quick Look and RealityKit

Balance the appearance and performance of your AR experiences with modeling strategies.

Adding an Apple Pay Button or a Custom Action in AR Quick Look

Provide a banner that users can tap to make a purchase or perform a custom action in an AR experience.

class ARQuickLookPreviewItem

An object for customizing the AR Quick Look experience.

USDZ schemas for AR

Add augmented reality functionality to your 3D content using USDZ schemas.

Specifying a lighting environment in AR Quick Look

Add metadata to your USDZ file to specify its lighting characteristics.

### Shared Experiences

Communicate with other devices to create a shared AR experience.

Streaming an AR experience

Control an AR experience remotely by transferring sensor and user input over the network.

Creating a collaborative session

Enable nearby devices to share an AR experience by using a peer-to-peer multiuser strategy.

Creating a multiuser AR experience

Enable nearby devices to share an AR experience by using a host-guest multiuser strategy.

class ARParticipantAnchor

An anchor for another user in multiuser augmented reality experiences.

class CollaborationData

An object that holds information that a user has collected about the physical environment.

### Audio

Creating an immersive ar experience with audio

Use sound effects and environmental sound layers to create an engaging AR experience.

### Errors

struct ARError

An error reported by ARKit.

enum Code

Codes that identify errors in ARKit.

## See Also

### iOS

Verifying Device Support and User Permission

Check whether your app can use ARKit and respect user privacy at runtime.

class ARSession

The object that manages the major tasks associated with every AR experience, such as motion tracking, camera passthrough, and image analysis.

class ARAnchor

An object that specifies the position and orientation of an item in the physical environment.

