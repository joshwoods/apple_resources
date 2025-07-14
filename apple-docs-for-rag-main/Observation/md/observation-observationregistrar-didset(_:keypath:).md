

- Observation
- ObservationRegistrar
-  didSet(\_:keyPath:) 

Instance Method

# didSet(\_:keyPath:)

A property observation called after setting the value of the subject.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func didSet(
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

### Receiving change notifications

func willSet&lt;Subject, Member>(Subject, keyPath: KeyPath&lt;Subject, Member>)

A property observation called before setting the value of the subject.

