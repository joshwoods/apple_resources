

- Core Data
- NSCustomMigrationStage
-  init(migratingFrom:to:) 

Initializer

# init(migratingFrom:to:)

Creates a custom migration stage with the specified source and destination model references.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+Swift 5.8+

``` source
convenience init(
    migratingFrom currentModel: NSManagedObjectModelReference,
    to nextModel: NSManagedObjectModelReference
)
```

## Parameters 

`currentModel`  

The reference that represents the migration’s source model.

`nextModel`  

The reference that represents the migration’s destination model.

## See Also

### Creating a custom migration stage

class NSManagedObjectModelReference

An object that describes a specific version of an object model.

