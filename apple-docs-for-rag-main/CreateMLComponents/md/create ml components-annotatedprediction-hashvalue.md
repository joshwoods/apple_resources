

- Create ML Components
- AnnotatedPrediction
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
var hashValue: Int { get }
```

Available when `Prediction` conforms to `Hashable` and `Annotation` conforms to `Hashable`.

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

