

- SwiftData
- PersistentModel
-  getValue(forKey:) 

Instance Method

# getValue(forKey:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func getValue(forKey: KeyPath) -> Value where Value : PersistentModel
```

## See Also

### Accessing a value by key path

func getValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self, Value>) -> Value

func getValue&lt;Value>(forKey: KeyPath&lt;Self, Value>) -> Value

func getValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self, Value>) -> Value

func getValue&lt;Value>(forKey: KeyPath&lt;Self, Value?>) -> Value?

func getTransformableValue&lt;Value>(forKey: KeyPath&lt;Self, Value>) -> Value

