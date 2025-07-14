

- SceneKit
- SCNScene
-  SCNScene.Attribute 

Structure

# SCNScene.Attribute

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct Attribute
```

## Topics

### Type Properties

static let endTime: SCNScene.Attribute

static let frameRate: SCNScene.Attribute

A floating-point value for the frame rate of the scene.

static let startTime: SCNScene.Attribute

static let upAxis: SCNScene.Attribute

An `SCNVector3` structure specifying the orientation of the scene.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Scene Attributes

func attribute(forKey: String) -> Any?

Returns the scene attribute for the specified key.

func setAttribute(Any?, forKey: String)

Sets a scene attribute for the specified key.

