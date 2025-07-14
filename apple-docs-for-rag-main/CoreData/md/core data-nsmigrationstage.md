

- Core Data
-  NSMigrationStage 

Class

# NSMigrationStage

An abstract base class for describing an individual stage of a migration.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class NSMigrationStage
```

## Overview

Important

Don’t create instances of NSMigrationStage. Instead, use a concrete subclass, such as NSLightweightMigrationStage or NSCustomMigrationStage.

## Topics

### Describing the purpose

var label: String!

The textual description of the migration stage’s purpose.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSCustomMigrationStage
- NSLightweightMigrationStage

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Migration stages

class NSLightweightMigrationStage

An object that describes a series of models suitable for lightweight migration.

class NSCustomMigrationStage

An object that enables you to participate in the migration between two versions of the same model.

