

- SwiftData
- PersistentModel
-  setValue(forKey:to:) 

Instance Method

# setValue(forKey:to:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func setValue(
    forKey: KeyPath,
    to newValue: Value
) where Value : PersistentModel
```

## See Also

### Modifying a value by key path

func setValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self, Value>, to: Value)

func setValue&lt;Value, OtherModel>(forKey: KeyPath&lt;Self, Value>, to: Value)

func setValue&lt;Value>(forKey: KeyPath&lt;Self, Value?>, to: Value?)

func setValue&lt;Value>(forKey: KeyPath&lt;Self, Value>, to: Value)

func setTransformableValue&lt;Value>(forKey: KeyPath&lt;Self, Value>, to: Value)

