

- SwiftData
-  Additional query macros 

API Collection

# Additional query macros

Supplementary macros that enable you to narrow query results and tell SwiftData how to sort and order those results.

## Topics

### Basic queries

macro Query(animation: Animation)

Fetches all instances of the attached model type, using the specified animation to animate any subsequent changes.

macro Query(transaction: Transaction)

Fetches all instances of the attached model type, using the specified transaction to animate any subsequent changes.

### Predicate-based queries

macro Query&lt;Element>(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], animation: Animation)

Fetches a sorted subset of the attached model type that satisfy the specified predicate.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, animation: Animation)

Fetches a subset of the attached model type, in a specific order, by sorting on a nonoptional attribute.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, animation: Animation)

Fetches a subset of the attached model type, in a specific order, by sorting on an optional attribute.

macro Query&lt;Element>(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], transaction: Transaction?)

Fetches and sorts the subset of the attached model type that satisfy the specified predicate.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, transaction: Transaction?)

Fetches a subset of the attached model type, in a specific order, by sorting on a nonoptional attribute.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, transaction: Transaction?)

Fetches a subset of the attached model type, in a specific order, by sorting on an optional attribute.

### Descriptor-based queries

macro Query&lt;Element>(FetchDescriptor&lt;Element>, animation: Animation)

Fetches only the subset of the attached model type that satisfy the provided fetch descriptor’s criteria.

macro Query&lt;Element>(FetchDescriptor&lt;Element>, transaction: Transaction?)

Fetches only the subset of the attached model type that satisfy the provided fetch descriptor’s criteria.

## See Also

### Model fetch

Filtering and sorting persistent data

Manage data store presentation using predicates and dynamic queries.

macro Query()

Fetches all instances of the attached model type.

struct Query

A type that fetches models using the specified criteria, and manages those models so they remain in sync with the underlying data.

struct FetchDescriptor

A type that describes the criteria, sort order, and any additional configuration to use when performing a fetch.

