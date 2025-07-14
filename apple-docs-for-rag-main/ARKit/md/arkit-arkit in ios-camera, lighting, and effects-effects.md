

- ARKit
- ARKit in iOS
-  Camera, Lighting, and Effects 

API Collection

# Camera, Lighting, and Effects

Determine the camera position and lighting for the current session, and apply effects, such as occlusion, to elements of the environment.

## Topics

### Camera

Get details about a user’s iOS device, like its position and orientation in 3D space, and the camera’s video data and exposure.

class ARCamera

Information about the camera position and imaging characteristics for a given frame.

### Lighting Effects

Adding realistic reflections to an AR experience

Use ARKit to generate environment probe textures from camera imagery and render reflective virtual objects.

class AREnvironmentProbeAnchor

An object that provides environmental lighting information for a specific area of space in a world-tracking AR session.

class ARLightEstimate

Estimated scene lighting information associated with a captured video frame in an AR session.

class ARDirectionalLightEstimate

Estimated environmental lighting information associated with a captured video frame in a face-tracking AR session.

### Occlusion

Occluding virtual content with people

Cover your app’s virtual content with people that ARKit perceives in the camera feed.

Effecting People Occlusion in Custom Renderers

Occlude your app’s virtual content where ARKit recognizes people in the camera feed by using matte generator.

Visualizing and interacting with a reconstructed scene

Estimate the shape of the physical environment using a polygonal mesh.

class ARMatteGenerator

An object that creates matte textures you use to occlude your app’s virtual content with people, that ARKit recognizes in the camera feed.

## See Also

### Virtual Content

Content Anchors

Identify items in the physical environment, including planar surfaces, images, physical objects, body positions, and faces.

Environmental Analysis

Analyze the video from the cameras and the accompanying data, and use ray-casting and depth-map information to determine the location of items.

Data Management

Obtain detailed information about skeletal and face geometry, and saved world data.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

