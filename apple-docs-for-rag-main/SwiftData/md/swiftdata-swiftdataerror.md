

- SwiftData
-  SwiftDataError 

Structure

# SwiftDataError

A type that describes a SwiftData error.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
struct SwiftDataError
```

## Topics

### Fetch errors

static let includePendingChangesWithBatchSize: SwiftDataError

static let sortingPendingChangesWithIdentifiers: SwiftDataError

static let unsupportedKeyPath: SwiftDataError

static let unsupportedPredicate: SwiftDataError

static let unsupportedSortDescriptor: SwiftDataError

### Configuration errors

static let configurationFileNameContainsInvalidCharacters: SwiftDataError

static let configurationFileNameTooLong: SwiftDataError

static let configurationSchemaNotFoundInContainerSchema: SwiftDataError

static let duplicateConfiguration: SwiftDataError

### Container errors

static let loadIssueModelContainer: SwiftDataError

### Context errors

static let modelValidationFailure: SwiftDataError

static let missingModelContext: SwiftDataError

### Migration errors

static let backwardMigration: SwiftDataError

static let unknownSchema: SwiftDataError

### Operators

static func == (SwiftDataError, SwiftDataError) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func ~= (SwiftDataError, any Error) -> Bool

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let historyTokenExpired: SwiftDataError

static let invalidTransactionFetchRequest: SwiftDataError

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum DataStoreError

A type that describes a data store error.

