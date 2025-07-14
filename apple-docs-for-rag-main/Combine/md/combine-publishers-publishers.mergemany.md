

- Combine
- Publishers
-  Publishers.MergeMany 

Structure

# Publishers.MergeMany

A publisher created by applying the merge function to an arbitrary number of upstream publishers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct MergeMany where Upstream : Publisher
```

## Topics

### Creating a Merge Many Publisher

init(Upstream...)

Creates a publisher created by applying the merge function to an arbitrary number of upstream publishers.

init&lt;S>(S)

Creates a publisher created by applying the merge function to a sequence of upstream publishers.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let publishers: [Upstream]

The array of upstream publishers that this publisher merges together.

### Comparing Publishers

static func == (Publishers.MergeMany&lt;Upstream>, Publishers.MergeMany&lt;Upstream>) -> Bool

Returns a Boolean value that indicates whether two publishers are equivalent.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Equatable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Publisher

## See Also

### Combining Elements from Multiple Publishers

struct CombineLatest

A publisher that receives and combines the latest elements from two publishers.

struct CombineLatest3

A publisher that receives and combines the latest elements from three publishers.

struct CombineLatest4

A publisher that receives and combines the latest elements from four publishers.

struct Merge

A publisher created by applying the merge function to two upstream publishers.

struct Merge3

A publisher created by applying the merge function to three upstream publishers.

struct Merge4

A publisher created by applying the merge function to four upstream publishers.

struct Merge5

A publisher created by applying the merge function to five upstream publishers.

struct Merge6

A publisher created by applying the merge function to six upstream publishers.

struct Merge7

A publisher created by applying the merge function to seven upstream publishers.

struct Merge8

A publisher created by applying the merge function to eight upstream publishers.

struct Zip

A publisher created by applying the zip function to two upstream publishers.

struct Zip3

A publisher created by applying the zip function to three upstream publishers.

struct Zip4

A publisher created by applying the zip function to four upstream publishers.

