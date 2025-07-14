

- SceneKit
-  SCNSkinner 

Class

# SCNSkinner

An object that manages the relationship between skeletal animations and the nodes and geometries they animate.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
class SCNSkinner
```

## Overview

Skeletal animation is a technique for simplifying the animation of complex geometries, such as humanoid characters in a game. An animation skeleton is a simple hierarchy of control nodes, which themselves have no visible geometry. Associating the skeleton with a geometry (also called “skinning” the skeleton or creating a skinned model) allows SceneKit to automatically deform the geometry when you move the skeleton’s control nodes, as shown below.

### Working with an Animation Skeleton

Typically, an artist creates a skinned model using external 3D authoring tools and saves it, along with animations that use the skeleton, in a scene file. You load the model from the scene file and pose or animate it in your app, either by using animation objects also loaded from the scene file or by directly manipulating the nodes in the skeleton.

You can also create a skinned model from separately defined geometry and skeleton data using the init(baseGeometry:bones:boneInverseBindTransforms:boneWeights:boneIndices:) method.

### Sharing a Skinner Object

To work with a skinned model’s skeleton, use the skinner property of the model’s root node. For example, one file might contain an animated game character, and other files might contain accessories (such as hats or backpacks) for the character to wear. An artist using 3D authoring tools can specify that the character and the accessories be animated using identical skeletons. To attach a hat to the character so that they animate together, you link the skinner object responsible for animating the hat to the skeleton associated with the animated character, as in the following example:

```
SCNNode *hero = [SCNScene sceneNamed:@"Hero"].rootNode;
SCNNode *hat = [SCNScene sceneNamed:@"FancyFedora"].rootNode;
hat.skinner.skeleton = hero.skinner.skeleton;
```

## Topics

### Creating a Skinner Object

convenience init(baseGeometry: SCNGeometry?, bones: [SCNNode], boneInverseBindTransforms: [NSValue]?, boneWeights: SCNGeometrySource, boneIndices: SCNGeometrySource)

Creates a skinner object with the specified visible geometry and skeleton information.

### Working with a Skinned Geometry

var baseGeometry: SCNGeometry?

The geometry whose surface the skinner’s animation skeleton deforms.

var baseGeometryBindTransform: SCNMatrix4

The coordinate transformation for the skinner’s geometry in its default state.

### Working with an Animation Skeleton

var skeleton: SCNNode?

The root node of the skinner object’s animation skeleton.

var bones: [SCNNode]

The control nodes of the animation skeleton.

var boneInverseBindTransforms: [NSValue]?

The default transforms for the animation skeleton’s bone nodes.

var boneWeights: SCNGeometrySource

The geometry source that defines the influence of each bone on the positions the geometry’s vertices.

var boneIndices: SCNGeometrySource

The geometry source defining the mapping from bone indices in skeleton data to the skinner’s bones array.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Animation and Constraints

Animation

Create declarative animations that move elements of a scene in predetermined ways, or manage animations imported with external authoring tools.

Constraints

Automatically adjust the position or orientation of a node based on specified rules.

class SCNMorpher

An object that manages smooth transitions between a node’s base geometry and one or more target geometries.

