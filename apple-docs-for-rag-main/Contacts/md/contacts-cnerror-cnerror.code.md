

- Contacts
- CNError
-  CNError.Code 

Enumeration

# CNError.Code

Error codes that the system may return when you use Contacts framework methods.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
enum Code
```

## Topics

### Errors

case authorizationDenied

An error that indicates the system denied authorization.

case changeHistoryExpired

An error that indicates the change history expired.

case changeHistoryInvalidAnchor

An error that indicates a change history anchor is invalid.

case changeHistoryInvalidFetchRequest

An error that indicates a change history fetch request is invalid.

case clientIdentifierCollision

An error that indicates a client identifier collision.

case clientIdentifierInvalid

An error that indicates the client identifier is invalid.

case clientIdentifierDoesNotExist

An error that indicates the client identifier doesn’t exist.

case communicationError

An error that indicates a communication error occurred.

case containmentCycle

An error with the containment cycle.

case containmentScope

An error with containment scope.

case dataAccessError

An error with data access.

case featureDisabledByUser

An error that indicates the user disabled the feature.

case featureNotAvailable

An error that indicates the feature isn’t available.

case insertedRecordAlreadyExists

An error that indicates the inserted record already exists.

case noAccessableWritableContainers

An error that indicates there are no accessible writable containers.

case parentContainerNotWritable

An error that indicates the parent container isn’t writable.

case parentRecordDoesNotExist

An error that indicates the parent record doesn’t exist.

case policyViolation

An error that indicates a policy violation.

case predicateInvalid

An error that indicates an invalid predicate.

case recordDoesNotExist

An error that indicates a record doesn’t exist.

case recordIdentifierInvalid

An error that indicates a record identifier is invalid.

case recordNotWritable

An error that indicates a record isn’t writable.

case unauthorizedKeys

An error that indicates unauthorized keys usage.

case validationMultipleErrors

An error that indicates the system encountered multiple validation errors.

case validationTypeMismatch

A validation error that indicates a type mismatch.

case validationConfigurationError

An error with validation configuration.

case vCardMalformed

An error that indicates a malformed vCard.

case vCardSummarizationError

An error that indicates a vCard summarization problem.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Error codes

struct CNError

Error information that may be returned when using the methods of the Contacts framework.

