

- Contacts
-  CNError 

Structure

# CNError

Error information that may be returned when using the methods of the Contacts framework.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
struct CNError
```

## Topics

### Error codes

static var authorizationDenied: CNError.Code

An error that indicates the system denied authorization.

static var changeHistoryExpired: CNError.Code

An error that indicates the change history expired.

static var changeHistoryInvalidAnchor: CNError.Code

An error that indicates a change history anchor is invalid.

static var changeHistoryInvalidFetchRequest: CNError.Code

An error that indicates a change history fetch request is invalid.

static var clientIdentifierCollision: CNError.Code

An error that indicates a client identifier collision.

static var clientIdentifierDoesNotExist: CNError.Code

An error that indicates the client identifier doesn’t exist.

static var clientIdentifierInvalid: CNError.Code

An error that indicates the client identifier is invalid.

static var communicationError: CNError.Code

An error that indicates a communication error occurred.

static var containmentCycle: CNError.Code

An error with the containment cycle.

static var containmentScope: CNError.Code

An error with containment scope.

static var dataAccessError: CNError.Code

An error with data access.

static var featureDisabledByUser: CNError.Code

An error that indicates the user disabled the feature.

static var featureNotAvailable: CNError.Code

An error that indicates the feature isn’t available.

static var insertedRecordAlreadyExists: CNError.Code

An error that indicates the inserted record already exists.

static var noAccessableWritableContainers: CNError.Code

An error that indicates there are no accessible writable containers.

static var parentContainerNotWritable: CNError.Code

An error that indicates the parent container isn’t writable.

static var parentRecordDoesNotExist: CNError.Code

An error that indicates the parent record doesn’t exist.

static var policyViolation: CNError.Code

An error that indicates a policy violation.

static var predicateInvalid: CNError.Code

An error that indicates an invalid predicate.

static var recordDoesNotExist: CNError.Code

An error that indicates a record doesn’t exist.

static var recordIdentifierInvalid: CNError.Code

An error that indicates a record identifier is invalid.

static var recordNotWritable: CNError.Code

An error that indicates a record isn’t writable.

static var unauthorizedKeys: CNError.Code

An error that indicates unauthorized keys usage.

static var vCardMalformed: CNError.Code

An error that indicates a malformed vCard.

static var vCardSummarizationError: CNError.Code

An error that indicates a vCard summarization problem.

static var validationConfigurationError: CNError.Code

An error with validation configuration.

static var validationMultipleErrors: CNError.Code

An error that indicates the system encountered multiple validation errors.

static var validationTypeMismatch: CNError.Code

A validation error that indicates a type mismatch.

### Error details

var affectedRecordIdentifiers: [String]?

An array of strings that uniquely identify the records affected by the error.

var affectedRecords: [AnyObject]?

An array of record objects for which the error applies.

enum Code

Error codes that the system may return when you use Contacts framework methods.

var keyPaths: [String]?

An array of key paths associated with the error.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Error codes

enum Code

Error codes that the system may return when you use Contacts framework methods.

