

- SwiftData
- MigrationStage
-  MigrationStage.custom(fromVersion:toVersion:willMigrate:didMigrate:) 

Case

# MigrationStage.custom(fromVersion:toVersion:willMigrate:didMigrate:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
case custom(
    fromVersion: any VersionedSchema.Type,
    toVersion: any VersionedSchema.Type,
    willMigrate: ((ModelContext) throws -> Void)?,
    didMigrate: ((ModelContext) throws -> Void)?
)
```

## See Also

### Migration stages

case lightweight(fromVersion: any VersionedSchema.Type, toVersion: any VersionedSchema.Type)

