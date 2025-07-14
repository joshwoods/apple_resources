

- Foundation
-  NSKeyValueObservingCustomization 

Protocol

# NSKeyValueObservingCustomization

Conforming to NSKeyValueObservingCustomization is not required to use Key-Value Observing. Provide an implementation of these functions if you need to disable auto-notifying for a key, or add dependent keys

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSKeyValueObservingCustomization : NSObjectProtocol
```

## Topics

### Type Methods

static func automaticallyNotifiesObservers(for: AnyKeyPath) -> Bool

**Required**

static func keyPathsAffectingValue(for: AnyKeyPath) -> Set&lt;AnyKeyPath>

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Protocols

protocol DiscreteFormatStyle

