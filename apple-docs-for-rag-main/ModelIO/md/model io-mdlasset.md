

- Model I/O
-  MDLAsset 

Class

# MDLAsset

An indexed container for 3D objects and associated information, such as transform hierarchies, meshes, cameras, and lights.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLAsset
```

## Overview

You create a MDLAsset object by loading data from a URL, and you can export an asset to any of several file formats. To access the objects contained in an asset, use Fast Enumeration, the object(at:) method, or subscripting. Each object in an asset can be the root of a hierarchy of objects. To traverse that hierarchy, use an object’s children property.

An asset may contain timed information, such as a series of mesh morphs. In such cases, the asset’s frameInterval property is nonzero and the startTime and endTime properties indicate the range of sample times available in the asset data. For objects contained in the asset, you can use methods such as localTransform(atTime:) and boundingBox(atTime:) to access object properties at a specific time sample. Requesting a sample outside the time range clamps to the start or end sample. Some asset formats support continuous sampling with interpolation for times between the samples stored in the asset; other asset formats are discrete. For an asset with discrete time information, requesting a sample time that falls between the samples stored in the asset returns data for the immediately preceding time.

## Topics

### Creating an Asset

class func canImportFileExtension(String) -> Bool

Returns a Boolean value that indicates whether the MDLAsset class can read asset data from files with the specified extension.

init(url: URL)

Initializes an asset from the file at the specified URL.

init(bufferAllocator: (any MDLMeshBufferAllocator)?)

Initializes an empty asset, using the specified buffer allocator.

init(url: URL?, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?)

Initializes an asset from the file at the specified URL, using the specified vertex descriptor and buffer allocator.

init(url: URL, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?, preserveTopology: Bool, error: NSErrorPointer)

Initializes an asset from the file at the specified URL, using the specified options for allocating and transforming data during import.

### Exporting an Asset

class func canExportFileExtension(String) -> Bool

Returns a Boolean value that indicates whether the MDLAsset class can write asset data as a file with the specified format extension.

func export(to: URL) throws

Writes asset data to a file at the specified URL and reports errors that occur during export.

### Working with Asset Content

func object(at: Int) -> MDLObject

Returns the top-level object at the specified index in the asset.

subscript(Int) -> MDLObject?

Returns the top-level object at the specified index in the asset, using subscript syntax.

var count: Int

The number of top-level objects in the asset.

func childObjects(of: AnyClass) -> [MDLObject]

Returns all objects contained in the asset of the specified class.

func add(MDLObject)

Adds the specified object to the asset’s list of top-level objects.

func remove(MDLObject)

Removes the specified object from the asset’s list of top-level objects.

var boundingBox: MDLAxisAlignedBoundingBox

The minimum region entirely enclosing the asset’s contents.

func boundingBox(atTime: TimeInterval) -> MDLAxisAlignedBoundingBox

Returns the minimum region entirely enclosing the asset’s contents at the specified time sample.

var url: URL?

The URL from which the asset was loaded, if available.

var bufferAllocator: any MDLMeshBufferAllocator

An object responsible for allocating mesh vertex data loaded from the asset.

var vertexDescriptor: MDLVertexDescriptor?

The description of the vertex data format to be used for loading mesh data from the asset.

var masters: any MDLObjectContainerComponent

An array of objects that can be reused in the asset’s object hierarchy through instancing.

Deprecated

### Working with Timed Information

var frameInterval: TimeInterval

The time interval between data samples in the asset.

var startTime: TimeInterval

The timestamp for the first timed data sample in the asset.

var endTime: TimeInterval

The timestamp for the last timed data sample in the asset.

### Working with Lights

class func placeLightProbes(withDensity: Float, heuristic: MDLProbePlacement, using: any MDLLightProbeIrradianceDataSource) -> [MDLLightProbe]

Automatically creates and places light probes for use in illuminating a scene.

enum MDLProbePlacement

Options affecting automatic placement of light probes in a scene, used with the placeLightProbes(withDensity:heuristic:using:) method.

### Constants

Asset File Types

Uniform Type Identifiers for file formats supported by the Model I/O framework.

### Instance Properties

var animations: any MDLObjectContainerComponent

var originals: any MDLObjectContainerComponent

var resolver: (any MDLAssetResolver)?

var upAxis: vector_float3

### Instance Methods

func loadTextures()

func object(atPath: String) -> MDLObject

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSFastEnumeration
- NSObjectProtocol

## See Also

### 3D Asset Basics

class MDLObject

The base class for objects that are part of a 3D asset, including meshes, cameras, and lights.

class MDLTransform

A description of the local coordinate space transformations for a 3D object.

class MDLMesh

A container for vertex buffer data to be used in rendering a 3D object.

class MDLSubmesh

A container for index buffer data and material information to be used in rendering all or part of a 3D object.

class MDLSubmeshTopology

A description of how a submesh’s index buffer data is arranged and how that arrangement should be used to produce the submesh’s intended 3D shape.

protocol MDLNamed

The common interface for Model I/O objects that expose a human-readable name.

