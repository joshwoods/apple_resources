

- Create ML
- MLCreateError
-  MLCreateError.io(reason:) 

Case

# MLCreateError.io(reason:)

An error that indicates an I/O failure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
case io(reason: String)
```

## See Also

### Identifying errors

case cancelled

An error that indicates you canceled the training session.

case incompatibleParameters(parameter: String, originalValue: String, newValue: String)

An error that indicates the training session parameters are incompatible.

case modifiedTrainingData

An error that indicates the training data is different from the data when you created the session.

case type(reason: String)

An error that indicates a missing or incorrect type.

case generic(reason: String)

An error that indicates a failure not covered by one of the other errors.

let MLCreateErrorDomain: String

A global constant that defines the domain for Create ML errors.

