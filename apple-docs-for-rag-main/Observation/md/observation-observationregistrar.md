

- Observation
-  ObservationRegistrar 

Structure

# ObservationRegistrar

Provides storage for tracking and access to data changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ObservationRegistrar
```

## Overview

You don’t need to create an instance of `ObservationRegistrar` when using the Observable() macro to indicate observability of a type.

## Topics

### Creating an observation registrar

init()

Creates an instance of the observation registrar.

### Receiving change notifications

func willSet&lt;Subject, Member>(Subject, keyPath: KeyPath&lt;Subject, Member>)

A property observation called before setting the value of the subject.

func didSet&lt;Subject, Member>(Subject, keyPath: KeyPath&lt;Subject, Member>)

A property observation called after setting the value of the subject.

### Identifying transactional access

func access&lt;Subject, Member>(Subject, keyPath: KeyPath&lt;Subject, Member>)

Registers access to a specific property for observation.

func withMutation&lt;Subject, Member, T>(of: Subject, keyPath: KeyPath&lt;Subject, Member>, () throws -> T) rethrows -> T

Identifies mutations to the transactions registered for observers.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Change tracking

func withObservationTracking&lt;T>(() -> T, onChange: @autoclosure () -> () -> Void) -> T

Tracks access to properties.

