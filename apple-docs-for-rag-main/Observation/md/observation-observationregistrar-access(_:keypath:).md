

- Observation
- ObservationRegistrar
-  access(\_:keyPath:) 

Instance Method

# access(\_:keyPath:)

Registers access to a specific property for observation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func access(
    _ subject: Subject,
    keyPath: KeyPath
) where Subject : Observable
```

## Parameters 

`subject`  

An instance of an observable type.

`keyPath`  

The key path of an observed property.

## See Also

### Identifying transactional access

func withMutation&lt;Subject, Member, T>(of: Subject, keyPath: KeyPath&lt;Subject, Member>, () throws -> T) rethrows -> T

Identifies mutations to the transactions registered for observers.

