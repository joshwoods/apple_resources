

- Assignables
-  AssignedWorkDocumentConfiguration 

Protocol

# AssignedWorkDocumentConfiguration

A type that specifies the score of a document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
protocol AssignedWorkDocumentConfiguration : Hashable
```

## Topics

### Configuring the score

var manualScore: Double?

An optional manual score for this work. If `nil`, the work score can be synthesized from the question data and associated annotations.

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable

## See Also

### Configuration

protocol AssignableDocumentConfiguration

A type that specifies the options for an assignable document.

