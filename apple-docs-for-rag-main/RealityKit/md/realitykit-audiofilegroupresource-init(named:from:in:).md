

- RealityKit
- AudioFileGroupResource
-  init(named:from:in:) 

Initializer

# init(named:from:in:)

Initializes an audio resource from a Reality Composer Pro project.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(
    named name: String,
    from scene: String,
    in bundle: Bundle
) async throws
```

## Parameters 

`name`  

The USD Prim path to the resource in the Reality Composer Pro project to initialize.

`scene`  

The name of the Reality Composer Pro scene to initialize from.

`bundle`  

The bundle that contains the project.

## Discussion

This method initializes a preconfigured AudioFileGroupResource from a scene in a Reality Composer Pro project.

Important

The name provided **must** be unique.

## See Also

### Creating a resource

init([AudioFileResource]) throws

Creates a group resource from an array of audio file resources.

static func load(named: String, from: String, in: Bundle?) throws -> AudioFileGroupResource

Loads an audio resource from a Reality Composer Pro project.

