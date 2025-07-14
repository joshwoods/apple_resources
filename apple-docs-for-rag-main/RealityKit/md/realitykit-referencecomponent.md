

- RealityKit
-  ReferenceComponent 

Structure

# ReferenceComponent

A component that can load another entity from a file.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ReferenceComponent
```

## Overview

You can use a `ReferenceComponent` to load other entities from files in your app’s main bundle. This allows you to load complex scenes incrementally, resulting in more responsive apps. It also enables collaborative workflows so you can split a complex scene into separate pieces that different teams own.

Use a `ReferenceComponent` by adding it to an entity when building up a scene programmatically. Then call write(to:) to save the scene to a `.reality` file.

```
// Create the root entity.
let root = Entity()

// Create an entity that references another entity file.
let earth = Entity()
earth.setParent(root)

// Add a reference to another entity that loads immediately
// when the root entity loads.
earth.components.set(ReferenceComponent(
    named: "Earth",
    loadingPolicy: .immediate))

// Add a reference to another entity that loads on demand.
let mars = Entity()
mars.name = "mars"
mars.components.set(ReferenceComponent(
    named: "Mars",
    loadingPolicy: .onDemand))

// Write the root entity to a `.reality` file.
try await root.write(to: fileURL)
```

When your app loads the `.reality` file, it can dynamically load referenced entities from files. For references that have a ReferenceComponent.LoadingPolicy of ReferenceComponent.LoadingPolicy.onDemand, you can use loadReference(at:) to load content on demand.

```
if let entity = root.findEntity(named: "mars") {
    try ReferenceComponent.loadReference(at: entity)
}
```

Conversely, use releaseReference(at:) to unload content and free up memory.

## Topics

### Initializers

init(named: String, at: String, loadingPolicy: ReferenceComponent.LoadingPolicy)

Creates a reference component with a name, loading policy, and bundle path.

init(named: String, in: Bundle, loadingPolicy: ReferenceComponent.LoadingPolicy)

Creates a reference component with a name, loading policy, and bundle.

init(named: String, loadingPolicy: ReferenceComponent.LoadingPolicy)

Creates a reference component with a name and loading policy.

### Instance Properties

var loadingPolicy: ReferenceComponent.LoadingPolicy

A policy that defines when a referenced entity loads.

var reference: Entity?

The root entity of the referenced entity file.

var state: ReferenceComponent.ReferenceState

A variable that indicates the loading state of the referenced entity.

### Type Methods

static func loadReference(at: Entity) async throws

Asynchronously loads another entity file that an entity depends on.

static func loadReference(at: Entity) throws

Synchronously loads another entity file that an entity depends on.

static func releaseReference(at: Entity) throws

Releases the reference an entity holds.

### Enumerations

enum LoadingPolicy

Describes when a referenced entity loads.

enum ReferenceState

Defines the current loading state of the referenced entity.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Loading an entity from a file

Loading entities from a file

Retrieve an entity from storage on disk using a synchronous or an asynchronous load operation.

Stored entities

Manage entities that you store as assets on disk.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

convenience init(contentsOf: URL, withName: String?) async throws

Creates an entity by asynchronously loading it from a file URL.

convenience init(named: String, in: Bundle?) async throws

Creates an entity by asynchronously loading it from a bundle.

