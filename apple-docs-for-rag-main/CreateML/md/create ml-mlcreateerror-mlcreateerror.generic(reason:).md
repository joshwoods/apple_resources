

- Create ML
- MLCreateError
-  MLCreateError.generic(reason:) 

Case

# MLCreateError.generic(reason:)

An error that indicates a failure not covered by one of the other errors.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
case generic(reason: String)
```

## See Also

### Identifying errors

case cancelled

An error that indicates you canceled the training session.

case incompatibleParameters(parameter: String, originalValue: String, newValue: String)

An error that indicates the training session parameters are incompatible.

case modifiedTrainingData

An error that indicates the training data is different from the data when you created the session.

case io(reason: String)

An error that indicates an I/O failure.

case type(reason: String)

An error that indicates a missing or incorrect type.

let MLCreateErrorDomain: String

A global constant that defines the domain for Create ML errors.

