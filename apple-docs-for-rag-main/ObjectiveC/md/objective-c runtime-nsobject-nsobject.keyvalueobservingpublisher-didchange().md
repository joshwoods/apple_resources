

- Objective-C Runtime
- NSObject
- NSObject.KeyValueObservingPublisher
-  didChange() 

Instance Method

# didChange()

Returns a publisher that emits values when a KVO-compliant property changes.

Objective-C RuntimeFoundationiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func didChange() -> Publishers.Map, Void>
```

Available when `Subject` inherits `NSObject`.

## Return Value

A key-value observing publisher.

