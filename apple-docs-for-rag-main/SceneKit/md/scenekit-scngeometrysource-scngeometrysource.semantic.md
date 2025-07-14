

- SceneKit
- SCNGeometrySource
-  SCNGeometrySource.Semantic 

Structure

# SCNGeometrySource.Semantic

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct Semantic
```

## Topics

### Basic Geometry Semantics

static let vertex: SCNGeometrySource.Semantic

The semantic for vertex position data.

static let normal: SCNGeometrySource.Semantic

The semantic for surface normal data.

static let texcoord: SCNGeometrySource.Semantic

The semantic for texture coordinate data.

### Advanced Shading Semantics

static let color: SCNGeometrySource.Semantic

The semantic for per-vertex color data.

static let tangent: SCNGeometrySource.Semantic

The semantic for surface tangent vector data.

### Surface Subdivision Semantics

static let edgeCrease: SCNGeometrySource.Semantic

The semantic for edge crease data, used for subdividing surfaces.

static let vertexCrease: SCNGeometrySource.Semantic

The semantic for vertex crease data, used for subdividing surfaces.

### Skeletal Animation Semantics

static let boneIndices: SCNGeometrySource.Semantic

The semantic for bone index data, used for skeletal animation of skinned surfaces.

static let boneWeights: SCNGeometrySource.Semantic

The semantic for bone weight data, used for skeletal animation of skinned surfaces.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

