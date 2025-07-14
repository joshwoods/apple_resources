

- Combine
- Publishers
- Publishers.Sequence
-  drop(while:) 

Instance Method

# drop(while:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func drop(while predicate: (Elements.Element) -> Bool) -> Publishers.Sequence, Failure>
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

