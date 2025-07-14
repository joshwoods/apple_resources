

- Core Data
- NSCustomMigrationStage
-  nextModel 

Instance Property

# nextModel

The reference that represents the migration’s destination model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var nextModel: NSManagedObjectModelReference { get }
```

## Discussion

Core Data sets this property to the `nextModel` parameter you specify when creating the migration stage.

## See Also

### Accessing model references

var currentModel: NSManagedObjectModelReference

The reference that represents the migration’s source model.

