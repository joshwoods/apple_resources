

- Core Data
- NSMigrationStage
-  label 

Instance Property

# label

The textual description of the migration stage’s purpose.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var label: String! { get set }
```

## Discussion

Persistent history tracking, if enabled, records the label for later use. The default value is an empty string.

