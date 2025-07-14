

- RealityKit
-  AudioLibraryComponent 

Structure

# AudioLibraryComponent

A container for audio resources that you can look up by user-defined names.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct AudioLibraryComponent
```

## Overview

`AudioLibraryComponent` serves as a container for audio resources, so that you can store loaded audio resources and associate them with an entity for playback using user-defined names. You may use any AudioResource type, such as AudioFileResource or AudioFileGroupResource.

Note

In memory, you can also use AudioBufferResource, but this type doesn’t support serializing to disk or sharing via network.

Below is an example of how you can set this component in code:

```
// Create a new entity.
let humanEntity = Entity()

// Set up two audio file resources, and combine them in one group resource.
let walkFileResource = try AudioFileResource.load(named: "HumanWalk")
let jumpFileResource = try AudioFileResource.load(named: "HumanJump")
let groupResource = try AudioFileGroupResource([walkFileResource, jumpFileResource])

// Create an `AudioLibraryComponent` to house the audio resources.
var audioLibraryComponent = AudioLibraryComponent()

// Add the resources to the component by name.
audioLibraryComponent.resources["Walk"] = walkFileResource
audioLibraryComponent.resources["Jump"] = jumpFileResource
audioLibraryComponent.resources["group"] = groupResource

humanEntity.components.set(audioLibraryComponent)

// Play the resource matching the "Walk" key on the entity -> Expect to play 'HumanWalk'.
humanEntity.playAudio(audioLibraryComponent.resources["Walk"]!)
```

By setting an `AudioLibraryComponent` on different entities, you can use simple defined names that trigger different sounds on different entities. For example, you can reuse the “Walk” string from the preceding example on a different entity:

```

// Create a new entity.
let robotEntity = Entity()

// Set up an audio file resource.
let robotWalkFileResource = try AudioFileResource.load(named: "RobotWalk")

// Create an `AudioLibraryComponent` to house the `audioResource`.
var audioLibraryComponent = AudioLibraryComponent()

// Add the resource to the component by name.
audioLibraryComponent.resources["Walk"] = robotWalkFileResource

robotEntity.components.set(audioLibraryComponent)

// Play the resource matching the "Walk" key on the entity -> Expect to play 'RobotWalk'.
robotEntity.playAudio(audioLibraryComponent.resources["Walk"]!)
```

Note

You can create a component using code, or add it to your entity using tools such as Reality Composer Pro.

In Reality Composer Pro, you can add an `AudioLibraryComponent` to an entity and then add audio resources to it for easy access to those resources by name. The system automatically loads the audio resources for you when you search for this component.

```
guard let audioLibraryComponent = entity.components[AudioLibraryComponent.self],
      let audioResource = audioLibraryComponent.resources["My_Audio_Resource_Name"]
else { return }

// Because the system has already loaded the resource for you,
// you may prepare or play it on an entity right away.
entity.playAudio(audioResource)
```

## Topics

### Creating an audio library component

init(resources: [String : AudioResource])

Creates a new audio library from a dictionary.

init(dictionaryLiteral: (String, AudioResource)...)

Creates an instance initialized with the given key-value pairs.

### Accessing audio resources

var resources: [String : AudioResource]

A dictionary of audio resources with user-defined names.

### Type Aliases

typealias Key

The key type of a dictionary literal.

typealias Value

The value type of a dictionary literal.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component
- ExpressibleByDictionaryLiteral

## See Also

### Audio resources

class AudioFileResource

An audio resource that you load from a file or from a URL.

class AudioFileGroupResource

An audio file group.

class AudioBufferResource

An audio resource that you load from an AVAudioBuffer.

class AudioResource

A playable audio resource

struct Calibration

A container for different calibration modes that can be applied for playback.

struct Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.

