

- Core Data
- NSCustomMigrationStage
-  currentModel 

Instance Property

# currentModel

The reference that represents the migration’s source model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var currentModel: NSManagedObjectModelReference { get }
```

## Discussion

Core Data sets this property to the `currentModel` parameter you specify when creating the migration stage.

## See Also

### Accessing model references

var nextModel: NSManagedObjectModelReference

The reference that represents the migration’s destination model.

