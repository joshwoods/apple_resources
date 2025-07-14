

- Combine
- Publishers
- Publishers.Sequence
-  filter(\_:) 

Instance Method

# filter(\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func filter(_ isIncluded: (Publishers.Sequence.Output) -> Bool) -> Publishers.Sequence.Output], Failure>
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

