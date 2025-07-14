

- Observation
- ObservationRegistrar
-  withMutation(of:keyPath:\_:) 

Instance Method

# withMutation(of:keyPath:\_:)

Identifies mutations to the transactions registered for observers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func withMutation(
    of subject: Subject,
    keyPath: KeyPath,
    _ mutation: () throws -> T
) rethrows -> T where Subject : Observable
```

## Parameters 

`subject`  

An instance of an observable type.

`keyPath`  

The key path of an observed property.

## Discussion

This method calls willSet(_:keyPath:) before the mutation. Then it calls didSet(_:keyPath:) after the mutation.

## See Also

### Identifying transactional access

func access&lt;Subject, Member>(Subject, keyPath: KeyPath&lt;Subject, Member>)

Registers access to a specific property for observation.

