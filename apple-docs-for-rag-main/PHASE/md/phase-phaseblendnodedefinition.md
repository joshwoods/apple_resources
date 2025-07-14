

- PHASE
-  PHASEBlendNodeDefinition 

Class

# PHASEBlendNodeDefinition

A node that smoothly fades between the audio of its child nodes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEBlendNodeDefinition
```

## Overview

This class defines a threshold and a numeric parameter the app increases and decreases to fade between child nodes. Each child node defines a range within the threshold in which the child node plays audio. As the app moves the blend parameter value between `0` and the threshold, the blend node plays the audio of its child nodes whose range and fade curve overlap at the current value.

### Play a Blend of Simultaneous Audio Data

To gradually change the audio that a sound event plays, define blend thresholds and a number metaparameter that incrementally increases or decreases between the thresholds. For example, the following code sets up a sound event hierarchy containing two sampler nodes that play audio, with each one modeling a different terrain. The app sets the metaparameter value based on the value of the terrain the player stands on. When the app starts a sound event from this hierarchy, PHASE plays:

- A grass footstep for terrain values between `0` and `0.33`

- A cobblestone footstep for terrain values between `0.67` and `1.0`

- A blend of both footstep sounds for values between `0.33` and `0.67`

```
// Create a meta parameter definition that chooses among different terrains.
let terrainBlendParameter = PHASENumberMetaParameterDefinition(
    value: 0.5, 
    minimum: 0.0,
    maximum: 1.0,
    identifier: "terrain")

// Create a blend node and pass in the meta parameter.
let terrainBlendNode = PHASEBlendNodeDefinition(blendMetaParameterDefinition: terrainBlendParameter)

// Add two samples nodes to blend between.
terrainBlendNode.addRangeForInputValuesAbove( 
    value: 0.33,
    fullGainAtValue: 1.0,
    fadeCurveType: .linear,
    subtree:cobblestoneSamplerNode)

terrainBlendNode.addRangeForInputValuesBelow( 
    value: 0.67,
    fullGainAtValue: 0.0,
    fadeCurveType: .linear,
    subtree:grassSamplerNode)

// Create a sound event.
var footstepEvent: PHASESoundEvent?
do { footstepEvent = try PHASESoundEvent(engine: myEngine, assetIdentifier: "terrain") } 
catch { fatalError("Failed to create the sound event due to: \(error)") }        

// Set the "terrain" metaparameter value to a midpoint that 
//  plays audio from both subtrees at an equal volume.
guard let terrainParameter = footstepEvent?.metaParameters["terrain"] else { fatalError() }
terrainParameter.value = 0.5

// Play the sound and hear a mix of both terrains.
footstepEvent?.start() { reason in 
/* Perform completion tasks. */ }
```

## Topics

### Creating a Blend Node

init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition)

Creates a blend node with a maxiumum blend range value.

convenience init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition, identifier: String)

Creates a named blend node with a maxiumum blend range value.

init(spatialMixerDefinition: PHASESpatialMixerDefinition)

Creates a blend node for spatial audio output.

convenience init(spatialMixerDefinition: PHASESpatialMixerDefinition, identifier: String)

Creates a named blend node for spatial audio output.

### Accessing Blend Properties

var blendParameterDefinition: PHASENumberMetaParameterDefinition?

The meta parameter definition that caps the blend range.

var spatialMixerDefinitionForDistance: PHASESpatialMixerDefinition?

An object that combines spatial audio layers.

### Adding Child Nodes

func addRange(envelope: PHASEEnvelope, subtree: PHASESoundEventNodeDefinition)

Adds a child node with an envelope.

func addRangeForInputValuesAbove(value: Double, fullGainAtValue: Double, fadeCurveType: PHASECurveType, subtree: PHASESoundEventNodeDefinition)

Adds a child node that blends above a given value.

func addRangeForInputValuesBelow(value: Double, fullGainAtValue: Double, fadeCurveType: PHASECurveType, subtree: PHASESoundEventNodeDefinition)

Adds a child node that blends below a given value.

func addRangeForInputValuesBetween(lowValue: Double, highValue: Double, fullGainAtLowValue: Double, fullGainAtHighValue: Double, lowFadeCurveType: PHASECurveType, highFadeCurveType: PHASECurveType, subtree: PHASESoundEventNodeDefinition)

Adds a child node that blends between a given high and low value.

## Relationships

### Inherits From

- PHASESoundEventNodeDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Control Nodes

class PHASESwitchNodeDefinition

A node that passes invocation to only one of its child nodes.

class PHASERandomNodeDefinition

A sound event node that invokes one of its child nodes at random.

class PHASEContainerNodeDefinition

A node that plays all its children at the same time.

