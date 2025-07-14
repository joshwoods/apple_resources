

- Combine
- Published
-  Published.Publisher 

Structure

# Published.Publisher

A publisher for properties marked with the `@Published` attribute.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Publisher
```

## Topics

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Instance Methods

func receive&lt;S>(subscriber: S)

Attaches the specified subscriber to this publisher.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Publishing the Value

var projectedValue: Published&lt;Value>.Publisher

The property for which this instance exposes a publisher.

