

- SwiftData
-  MigrationStage 

Enumeration

# MigrationStage

Describes a migration between two versions of the same schema.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
enum MigrationStage
```

## Topics

### Migration stages

case lightweight(fromVersion: any VersionedSchema.Type, toVersion: any VersionedSchema.Type)

case custom(fromVersion: any VersionedSchema.Type, toVersion: any VersionedSchema.Type, willMigrate: ((ModelContext) throws -> Void)?, didMigrate: ((ModelContext) throws -> Void)?)

## See Also

### Managing migration stages

static var stages: [MigrationStage]

**Required**

