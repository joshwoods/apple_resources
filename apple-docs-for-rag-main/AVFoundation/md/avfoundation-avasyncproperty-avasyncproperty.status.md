

- AVFoundation
- AVAsyncProperty
-  AVAsyncProperty.Status 

Enumeration

# AVAsyncProperty.Status

Loaded status values for asynchronous properties.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum Status
```

## Mentioned in 

Loading media data asynchronously

## Topics

### Status Values

case notYetLoaded

The system hasn’t loaded a property value.

case loading

The system is loading the property.

case loaded(Value)

A property value is ready to use.

case failed(NSError)

A property value fails to load.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

