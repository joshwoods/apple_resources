

- SwiftData
-  PersistentModel 

Protocol

# PersistentModel

An interface that enables SwiftData to manage a Swift class as a stored model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
protocol PersistentModel : AnyObject, Observable, Hashable, Identifiable
```

## Mentioned in 

Preserving your app’s model data across launches

## Topics

### Creating a persistent model

init(backingData: any BackingData&lt;Self>)

**Required**

### Identifying the model instance

var persistentModelID: PersistentIdentifier

struct PersistentIdentifier

A type that describes the aggregate identity of a SwiftData model.

var modelContext: ModelContext?

### Accessing a value by key path

func getValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self, Value>) -> Value

func getValue&lt;Value>(forKey: KeyPath&lt;Self, Value>) -> Value

func getValue&lt;Value>(forKey: KeyPath&lt;Self, Value>) -> Value

func getValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self, Value>) -> Value

func getValue&lt;Value>(forKey: KeyPath&lt;Self, Value?>) -> Value?

func getTransformableValue&lt;Value>(forKey: KeyPath&lt;Self, Value>) -> Value

### Modifying a value by key path

func setValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self, Value>, to: Value)

func setValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self, Value>, to: Value)

func setValue&lt;Value>(forKey: KeyPath&lt;Self, Value?>, to: Value?)

func setValue&lt;Value>(forKey: KeyPath&lt;Self, Value>, to: Value)

func setValue&lt;Value>(forKey: KeyPath&lt;Self, Value>, to: Value)

func setTransformableValue&lt;Value>(forKey: KeyPath&lt;Self, Value>, to: Value)

### Accessing supplementary information

static var schemaMetadata: [Schema.PropertyMetadata]

**Required**

var persistentBackingData: any BackingData&lt;Self>

**Required**

var hasChanges: Bool

var isDeleted: Bool

### Internal

Internal symbols

Restricted-use symbols that the framework requires for macro expansion and other internal tasks.

### Type Methods

static func createBackingData&lt;P>() -> some BackingData&lt;P> 

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Inherits From

- Equatable
- Hashable
- Identifiable
- Observable

## See Also

### Creating a model container

init(for: Schema, migrationPlan: (any SchemaMigrationPlan.Type)?, configurations: [ModelConfiguration]) throws

Creates a model container using the specified schema, migration plan, and configurations.

convenience init(for: any PersistentModel.Type..., migrationPlan: (any SchemaMigrationPlan.Type)?, configurations: ModelConfiguration...) throws

Creates a model container using the specified model types, migration plan, and zero or more configurations.

convenience init(for: Schema, migrationPlan: (any SchemaMigrationPlan.Type)?, configurations: ModelConfiguration...) throws

Creates a model container using the specified schema, migration plan, and zero or more configurations.

struct ModelConfiguration

A type that describes the configuration of an app’s schema or specific group of models.

class Schema

An object that maps model classes to data in the model store, and helps with the migration of that data between releases.

protocol SchemaMigrationPlan

An interface for describing the evolution of a schema and how to migrate between specific versions.

