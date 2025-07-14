

- PHASE
-  PHASERandomNodeDefinition 

Class

# PHASERandomNodeDefinition

A sound event node that invokes one of its child nodes at random.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASERandomNodeDefinition
```

## Overview

When the framework invokes a random node, it passes the invocation on to one of its children at random. The weight you choose for a child node in the addSubtree(_:weight:) argument skews the node’s selection chances.

### Choose from Alternate Sounds

This class can model real-world cases where an event varies slightly, such as when footsteps sound slightly different because of the unique ground composition at each step.

The following code creates an instance of this class that selects from three different footstep sounds. The weights determine that an uncommon footstep noise plays half as frequently as the common footstep. And a third footstep noise plays 10% of the time.

- Swift
- Objective-C

```
// Create several nodes from prior-registered footstep sound assets.
let footstep1 = PHASESamplerNodeDefinition(
    soundAssetIdentifier: "footstep1",
    mixerDefinition: myMixer, identifier: "footstep1")
let footstep2 = PHASESamplerNodeDefinition(
    soundAssetIdentifier: "footstep2",
    mixerDefinition: myMixer, identifier: "footstep2")
let footstep3 = PHASESamplerNodeDefinition(
    soundAssetIdentifier: "footstep3",    
    mixerDefinition: myMixer, identifier: "footstep3")

// Create the random node.
let randomNode = PHASERandomNodeDefinition(identifier: "randomNode")

// Connect leaf nodes to the tree and set the weights. 
randomNode.addSubtree(footstep1, weight: 10)
randomNode.addSubtree(footstep2, weight: 5)
randomNode.addSubtree(footstep3, weight: 1)
```

```
// Create several nodes from prior-registered footstep sound assets.
PHASESamplerNodeDefinition* footstep1 = 
    [[PHASESamplerNodeDefinition alloc] 
        initWithSoundAssetUID:@"footstep1" 
        mixerDefinition:mixNode uid:@"footstep1"];
PHASESamplerNodeDefinition* footstep2 = 
    [[PHASESamplerNodeDefinition alloc] 
        initWithSoundAssetUID:@"footstep2" 
        mixerDefinition:mixNode uid:@"footstep2"];
PHASESamplerNodeDefinition* footstep3 = 
    [[PHASESamplerNodeDefinition alloc] 
        initWithSoundAssetUID:@"footstep3" 
        mixerDefinition:mixNode uid:@"footstep3"];

// Create the random node.
PHASERandomNodeDefinition* randomNode = 
    [[PHASERandomNodeDefinition alloc] initWithUID:@"randomNode"];

// Connect leaf nodes to the tree and set the weights. 
[randomNode addSubtree:footstep1 weight:@10];
[randomNode addSubtree:footstep2 weight:@5];
[randomNode addSubtree:footstep3 weight:@1];
```

## Topics

### Creating a Node

init()

Creates a random node.

convenience init(identifier: String)

Creates a random node with the name you specify.

### Adding Descendent Nodes

func addSubtree(PHASESoundEventNodeDefinition, weight: NSNumber)

Adds a node tree that’s one of the random-selection options.

### Defining Selection Queue Length

var uniqueSelectionQueueLength: Int

The length of the unique selection queue.

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

class PHASEBlendNodeDefinition

A node that smoothly fades between the audio of its child nodes.

class PHASEContainerNodeDefinition

A node that plays all its children at the same time.

