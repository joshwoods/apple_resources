

- RealityKit
- Entity
-  Stored entities 

API Collection

# Stored entities

Manage entities that you store as assets on disk.

## Overview

If you bundle 3D assets with your app, or download them from the network into local file storage, you need a way to load them at runtime. RealityKit provides a collection of methods that you use to load USD and Reality files into Entity instances.

## Topics

### Essentials

Loading entities from a file

Retrieve an entity from storage on disk using a synchronous or an asynchronous load operation.

class LoadRequest

A resource loader that acts as a publisher.

Deprecated

### Loading an entity hierarchy

static func load(named: String, in: Bundle?) throws -> Entity

Returns an entity by synchronously loading it from a bundle.

static func load(contentsOf: URL, withName: String?) throws -> Entity

Returns an entity by synchronously loading it from a file URL.

static func loadAsync(named: String, in: Bundle?) -> LoadRequest&lt;Entity>

Returns a load request that creates an entity by asynchronously loading it from a bundle.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;Entity>

Returns a load request that creates an entity by asynchronously loading it from a file URL and preserving the entity’s hierarchy.

Deprecated

### Loading an anchor entity

static func loadAnchor(named: String, in: Bundle?) throws -> AnchorEntity

Synchronously loads an anchor entity from a bundle.

static func loadAnchor(contentsOf: URL, withName: String?) throws -> AnchorEntity

Synchronously loads an anchor entity from a file URL.

static func loadAnchorAsync(named: String, in: Bundle?) -> LoadRequest&lt;AnchorEntity>

Asynchronously loads an anchor entity from a bundle.

Deprecated

static func loadAnchorAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;AnchorEntity>

Asynchronously loads an anchor entity from a file URL.

Deprecated

### Loading a flattened model entity

static func loadModel(named: String, in: Bundle?) throws -> ModelEntity

Synchronously loads a model entity from a bundle.

static func loadModel(contentsOf: URL, withName: String?) throws -> ModelEntity

Synchronously loads a model entity from a file URL.

static func loadModelAsync(named: String, in: Bundle?) -> LoadRequest&lt;ModelEntity>

Asynchronously loads a model entity from a bundle.

Deprecated

static func loadModelAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;ModelEntity>

Returns a load request that creates a model entity by asynchronously loading it from a file URL and flattening the model entity’s hierarchy.

Deprecated

### Loading a flattened body-tracked entity

static func loadBodyTracked(named: String, in: Bundle?) throws -> BodyTrackedEntity

Synchronously loads a body-tracked entity from a bundle.

static func loadBodyTracked(contentsOf: URL, withName: String?) throws -> BodyTrackedEntity

Synchronously loads a body-tracked entity from a file URL.

static func loadBodyTrackedAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;BodyTrackedEntity>

Asynchronously loads a body-tracked entity from a file URL.

static func loadBodyTrackedAsync(named: String, in: Bundle?) -> LoadRequest&lt;BodyTrackedEntity>

Asynchronously loads a body-tracked entity from a bundle.

Deprecated

## See Also

### Loading an entity from a file

Loading entities from a file

Retrieve an entity from storage on disk using a synchronous or an asynchronous load operation.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

convenience init(contentsOf: URL, withName: String?) async throws

Creates an entity by asynchronously loading it from a file URL.

convenience init(named: String, in: Bundle?) async throws

Creates an entity by asynchronously loading it from a bundle.

struct ReferenceComponent

A component that can load another entity from a file.

