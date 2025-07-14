

- Core Data
-  NSManagedObjectModelReference 

Class

# NSManagedObjectModelReference

An object that describes a specific version of an object model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class NSManagedObjectModelReference
```

## Topics

### Creating a reference

init(model: NSManagedObjectModel, versionChecksum: String)

Creates an object model reference for the specified model.

init(fileURL: URL, versionChecksum: String)

Creates an object model reference for the model at the specified file URL.

init(name: String, in: Bundle?, versionChecksum: String)

Creates an object model reference for the named model in the specified bundle.

init(entityVersionHashes: [AnyHashable : Any], in: Bundle?, versionChecksum: String)

Creates an object model reference with the entities corresponding to the specified entity version hashes.

### Resolving the model object

var resolvedModel: NSManagedObjectModel

The resolved object model.

var versionChecksum: String

The version checksum of the resolved model.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating a custom migration stage

convenience init(migratingFrom: NSManagedObjectModelReference, to: NSManagedObjectModelReference)

Creates a custom migration stage with the specified source and destination model references.

