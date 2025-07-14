

- PHASE
-  PHASESwitchNodeDefinition 

Class

# PHASESwitchNodeDefinition

A node that passes invocation to only one of its child nodes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESwitchNodeDefinition
```

## Overview

A switch node takes a different path in a sound-event hierarchy depending on the value that the app supplies for the node’s switch metaparameter. You define the available paths ahead of time by calling addSubtree(_:switchValue:) at least twice and supplying the subtree’s unique string name as the switch value. When your app invokes a sound event at runtime, PHASE checks the value of switchMetaParameterDefinition to determine which path to take.

### Switch Between Mulitple Node Trees

For example, the following diagram represents a node tree that plays one of three grass or sidewalk footstep sounds, depending on the app’s current state. The app sets a value for the switch-node metaparameter according to the terrain on which the player in a game currently stands.

The following code creates a random node subtree for each terrain type and adds each one as a subtree to the switch node.

- Swift
- Objective-C

```
// Set up the sampler nodes for the "grass" group of sounds.
let grassFootstep1 = PHASESamplerNodeDefinition(soundAssetIdentifier:"GrassOne" , mixerDefinition: myMixer)
let grassFootstep2 = PHASESamplerNodeDefinition(soundAssetIdentifier:"GrassTwo" , mixerDefinition: myMixer)

// Create a random node and assign the grass samplers to it.
let grassRandomNode = PHASERandomNodeDefinition(identifier: "grassRandomNode")
grassRandomNode.addSubtree(grassFootstep1, weight: 10)
grassRandomNode.addSubtree(grassFootstep2, weight: 5)

// Set up the sampler nodes for the "cobblestone" group of sounds.
let cobblestoneFootstep1 = PHASESamplerNodeDefinition(soundAssetIdentifier: "CobblestoneOne", mixerDefinition: myMixer)
let cobblestoneFootstep2 = PHASESamplerNodeDefinition(soundAssetIdentifier: "CobblestoneTwo", mixerDefinition: myMixer)

// Create a random node and assign the cobblestone samplers to it.
let cobblestoneRandomNode = PHASERandomNodeDefinition(identifier: "cobblestoneRandomNode")
cobblestoneRandomNode.addSubtree(cobblestoneFootstep1, weight: 4)
cobblestoneRandomNode.addSubtree(cobblestoneFootstep2, weight: 2)

// Create a metaparameter definition named "terrain" for the sound event.
let terrainSwitchParameter = PHASEStringMetaParameterDefinition(value: "cobblestone", identifier:"terrain")

// Create a switch node and provide the metaparameter.
let terrainSwitchNode = PHASESwitchNodeDefinition(switchMetaParameterDefinition: terrainSwitchParameter)

// Add two random nodes as the metaparameter toggle options.
terrainSwitchNode.addSubtree(cobblestoneRandomNode, switchValue: "cobblestone")
terrainSwitchNode.addSubtree(grassRandomNode, switchValue: "grass")

// Set the terrain metaparameter to play the sound event.
var footstepEvent: PHASESoundEvent!
do {
    footstepEvent = try PHASESoundEvent(engine: myEngine, assetIdentifier: "footStepEventAsset")
} catch { fatalError("Failed to create sound event.") }

// Set the terrain to grass.
if let metaparameter = footstepEvent.metaParameters["terrain"] {
    metaparameter.value = "grass"
}

// Invoke the sound event and hear noise for the selected terrain.
footstepEvent.start()
```

```
// Set up the sampler nodes for the "grass" group of sounds.
PHASESamplerNodeDefinition* grassFootstep1 = [[PHASESamplerNodeDefinition alloc] 
    initWithSoundAssetUID:@"GrassOne" mixerDefinition:mixNode];
PHASESamplerNodeDefinition* grassFootstep2 = [[PHASESamplerNodeDefinition alloc] 
    initWithSoundAssetUID:@"GrassTwo" mixerDefinition:mixNode];

// Create a random node and assign the grass samplers to it.
PHASERandomNodeDefinition* grassRandomNode = [[PHASERandomNodeDefinition alloc] 
    initWithUID:@"grassRandomNode"];
[grassRandomNode addSubtree:grassFootstep1 weight:@10];
[grassRandomNode addSubtree:grassFootstep2 weight:@5];

// Set up the sampler nodes for the "cobblestone" group of sounds.
PHASESamplerNodeDefinition* cobblestoneFootstep1 = [[PHASESamplerNodeDefinition alloc] 
    initWithSoundAssetUID:@"CobblestoneOne" mixerDefinition:mixNode];
PHASESamplerNodeDefinition* cobblestoneFootstep2 = [[PHASESamplerNodeDefinition alloc] 
    initWithSoundAssetUID:@"CobblestoneTwo" mixerDefinition:mixNode];

// Create a random node and assign the cobblestone samplers to it.
PHASERandomNodeDefinition* cobblestoneRandomNode = [[PHASERandomNodeDefinition alloc] 
    initWithUID:@"cobblestoneRandomNode"];
[cobblestoneRandomNode addSubtree:cobblestoneFootstep1 weight:@4];
[cobblestoneRandomNode addSubtree:cobblestoneFootstep2 weight:@2];

// Create a metaparameter definition named "terrain" for the sound event.
PHASEStringMetaParameterDefinition terrainSwitchParameter = 
    [[PHASEStringMetaParameterDefinition alloc] 
        initWithValue:@"cobblestone" uid:@"terrain"];

// Create a switch node and provide the metaparameter.
PHASESwitchNodeDefinition* terrainSwitchNode = [[PHASESwitchNodeDefinition alloc] 
    initWithSwitchMetaParameterDefinition:terrainSwitchParameter];

// Add two random nodes as the metaparameter toggle options.
[terrainSwitchNode addSubtree:cobblestoneRandomNode switchValue:@"cobblestone"];
[terrainSwitchNode addSubtree:grassRandomNode switchValue:@"grass"];

// Set the terrain metaparameter to play the sound event.
PHASESoundEvent* footstepEvent = [[PHASESoundEvent alloc] 
    initWithEngine:_objects->mEngine
    registeredSoundEventNodeAssetUID:@"footStepEventAsset" outError:nil];

// Set the terrain to grass.
footstepEvent.metaParameters[@"terrain"] = @"grass";

// Invoke the sound event and hear noise for the selected terrain.
[footstepEvent startAndReturnError:&myError];
```

Tip

The metaParameters objects affect only one sound event. To propagate a metaparameter change to multiple sound events, register the metaparameter globally using registerGlobalMetaParameter(metaParameterDefinition:), and change its value through the asset registry’s globalMetaParameters dictionary.

## Topics

### Creating a Node

init(switchMetaParameterDefinition: PHASEStringMetaParameterDefinition)

Creates a node that invokes a child node based on the value of the given parameter.

convenience init(switchMetaParameterDefinition: PHASEStringMetaParameterDefinition, identifier: String)

Creates a named node that invokes a child node based on the value of the given parameter.

### Managing Child Nodes

var switchMetaParameterDefinition: PHASEStringMetaParameterDefinition

The meta parameter that holds the name of the child node to invoke.

func addSubtree(PHASESoundEventNodeDefinition, switchValue: String)

Adds a child node with the given switch value.

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

class PHASERandomNodeDefinition

A sound event node that invokes one of its child nodes at random.

class PHASEBlendNodeDefinition

A node that smoothly fades between the audio of its child nodes.

class PHASEContainerNodeDefinition

A node that plays all its children at the same time.

