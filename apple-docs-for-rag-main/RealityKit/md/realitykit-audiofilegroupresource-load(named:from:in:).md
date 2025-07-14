

- RealityKit
- AudioFileGroupResource
-  load(named:from:in:) 

Type Method

# load(named:from:in:)

Loads an audio resource from a Reality Composer Pro project.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static func load(
    named name: String,
    from scene: String,
    in bundle: Bundle? = nil
) throws -> AudioFileGroupResource
```

## Parameters 

`name`  

The USD Prim path to the resource in the Reality Composer Pro project to load.

`scene`  

The name of the Reality Composer Pro scene to load from.

`bundle`  

The bundle that contains the project. Leave `nil` to load from the app’s bundle.

## Discussion

This method loads a preconfigured AudioFileGroupResource from a scene in a Reality Composer Pro project.

Important

The name provided **must** be unique.

## See Also

### Creating a resource

init([AudioFileResource]) throws

Creates a group resource from an array of audio file resources.

convenience init(named: String, from: String, in: Bundle) async throws

Initializes an audio resource from a Reality Composer Pro project.

