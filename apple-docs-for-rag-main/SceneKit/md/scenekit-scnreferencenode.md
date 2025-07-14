

- SceneKit
-  SCNReferenceNode 

Class

# SCNReferenceNode

A scene graph node that serves as a placeholder for content to be loaded from a separate scene file.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
class SCNReferenceNode
```

**macOS, watchOS**

``` source
class SCNReferenceNode
```

## Overview

When you tell a reference node to load its content, SceneKit loads the referenced scene file and makes children of the scene file’s root node become children of the reference node.

## Topics

### Creating a Reference Node

init?(url: URL)

Initializes a node whose content is to be loaded from the referenced URL.

### Loading and Unloading a Reference Node’s Content

var referenceURL: URL

The URL to a scene file from which to load content for the reference node.

var loadingPolicy: SCNReferenceLoadingPolicy

An option for whether to load the node’s content automatically.

func load()

Loads content into the node from its referenced external scene file.

var isLoaded: Bool

A Boolean value that indicates whether the reference node has already loaded its content.

func unload()

Removes the node’s children and marks the node as not loaded.

### Constants

enum SCNReferenceLoadingPolicy

Options for when to load the reference node’s content, used by the loadingPolicy property.

### Initializers

init?(coder: NSCoder)

## Relationships

### Inherits From

- SCNNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- SCNActionable
- SCNAnimatable
- SCNBoundingVolume
- Sendable
- UIFocusEnvironment
- UIFocusItem

## See Also

### Scene Structure

Organizing a Scene with Nodes

Use nodes to define the structure of a scene.

class SCNNode

A structural element of a scene graph, representing a position and transform in a 3D coordinate space, to which you can attach geometry, lights, cameras, or other displayable content.

