

- SwiftData
-  BackingData 

Protocol

# BackingData

An interface for providing in-memory storage for a persistent model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
protocol BackingData
```

## Topics

### Associated Types

associatedtype Model : PersistentModel

**Required**

### Initializers

init(for: Self.Model.Type)

**Required**

### Instance Properties

var metadata: Any

**Required**

var persistentModelID: PersistentIdentifier?

**Required**

### Instance Methods

func getTransformableValue&lt;Value>(forKey: KeyPath&lt;Self.Model, Value>) -> Value

**Required**

func getValue&lt;Value>(forKey: KeyPath&lt;Self.Model, Value>) -> Value

**Required**

func getValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self.Model, Value>) -> Value

**Required**

func getValue&lt;Value>(forKey: KeyPath&lt;Self.Model, Value>) -> Value

**Required**

func getValue&lt;Value>(forKey: KeyPath&lt;Self.Model, Value?>) -> Value?

**Required**

func getValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self.Model, Value>) -> Value

**Required**

func setTransformableValue&lt;Value>(forKey: KeyPath&lt;Self.Model, Value>, to: Value)

**Required**

func setValue&lt;Value>(forKey: KeyPath&lt;Self.Model, Value>, to: Value)

**Required**

func setValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self.Model, Value>, to: Value)

**Required**

func setValue&lt;Value>(forKey: KeyPath&lt;Self.Model, Value>, to: Value)

**Required**

func setValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self.Model, Value>, to: Value)

**Required**

func setValue&lt;Value>(forKey: KeyPath&lt;Self.Model, Value?>, to: Value?)

**Required**

