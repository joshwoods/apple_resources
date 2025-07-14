

- RealityKit
- ARView
- ARView.DebugOptions
-  showStatistics 

Type Property

# showStatistics

Collect performance statistics and display them in the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
static let showStatistics: ARView.DebugOptions
```

## Discussion

Add this debug option to a view’s debugOptions option set to display a variety of resource utilization metrics, overlaid on the view. The statistics update in real time so you can examine how your app performs and what resources it consumes under different usage conditions.

For more information about how to use the data shown above and described below, see Improving the Performance of a RealityKit App.

### Measure time

Items listed under the Frame CPU Time heading show how your app makes use of CPU time. The first item indicates frame rate, which directly impacts the quality of the user’s experience. The remaining items indicate average time in milliseconds per frame that the CPU spends performing certain tasks, as described below.

FPS  
The number of rendered frames per second. Typically capped at 60 fps, the system might reduce the frame rate under certain conditions. To achieve 60 fps, complete all computations in under 16.6 ms.

Main Thread  
Time spent performing Entity Component System (ECS), physics, animation, networking, and other computations like app updates. The CPU also works on this thread to prepare data for the render thread.

Render Thread  
Time spent in the render thread. The CPU creates command buffers and encoders to send to the GPU for processing.

ECS  
Time spent updating all components in your scene, getting them ready for physics, network, animation, and other updates.

Physics  
Time spent resolving collisions and physics simulations per frame. Additional physics work takes places during the ECS time as well as part of component updates.

Network  
Time spent sending and receiving data. The creation and processing of network data is part of the ECS time.

Animation  
Time spent managing animations. Some animation tasks occur during component updates, so they contribute to the ECS time instead.

### Measure geometry

Items under the Scene Mesh Stats heading help you optimize your content. These statistics help you to estimate the complexity of your scene.

Meshes  
The number of meshes in the view. Reduce this number to lower both ECS and Render Thread times.

Draw Calls  
The number of draw calls required to render the scene. Reduce this number to lower the Render Thread time.

Triangles Submitted  
The number of triangles submitted to the GPU on each frame.

Vertices Submitted  
The number of vertices submitted to the GPU on each frame.

### Measure memory

The items under the App Memory Usage heading help you understand how much memory your app uses.

Dirty Memory Footprint  
The amount of memory your app uses per frame.

Peak Dirty Memory Footprint  
The worst case amount of memory your app uses per frame.

## See Also

### Configuring debug options

static let none: ARView.DebugOptions

Disable all debugging overlays.

static let showPhysics: ARView.DebugOptions

Draw visualizations for collision objects and rigid bodies.

static let showAnchorOrigins: ARView.DebugOptions

Display anchor origins.

static let showAnchorGeometry: ARView.DebugOptions

Display anchor geometry.

static let showWorldOrigin: ARView.DebugOptions

Display a coordinate axis indicating the position and orientation of the AR world coordinate system.

static let showFeaturePoints: ARView.DebugOptions

Display a point cloud showing intermediate results of the scene analysis used to track device position.

static let showSceneUnderstanding: ARView.DebugOptions

Display the depth-colored wireframe for scene-understanding meshes.

