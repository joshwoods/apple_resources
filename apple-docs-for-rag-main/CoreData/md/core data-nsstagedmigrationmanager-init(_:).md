

- Core Data
- NSStagedMigrationManager
-  init(\_:) 

Initializer

# init(\_:)

Creates a migration manager with the specified stages.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+Swift 5.8+

``` source
convenience init(_ stages: [NSMigrationStage])
```

## Parameters 

`stages`  

The array of migration stages to execute.

## Discussion

Important

Core Data processes the migration stages in the order that you provide them.

