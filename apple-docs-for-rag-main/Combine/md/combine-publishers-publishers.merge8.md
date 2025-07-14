

- Combine
- Publishers
-  Publishers.Merge8 

Structure

# Publishers.Merge8

A publisher created by applying the merge function to eight upstream publishers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Merge8 where A : Publisher, B : Publisher, C : Publisher, D : Publisher, E : Publisher, F : Publisher, G : Publisher, H : Publisher, A.Failure == B.Failure, A.Output == B.Output, B.Failure == C.Failure, B.Output == C.Output, C.Failure == D.Failure, C.Output == D.Output, D.Failure == E.Failure, D.Output == E.Output, E.Failure == F.Failure, E.Output == F.Output, F.Failure == G.Failure, F.Output == G.Output, G.Failure == H.Failure, G.Output == H.Output
```

## Topics

### Creating a Merge-Eight Publisher

init(A, B, C, D, E, F, G, H)

Creates a publisher created by applying the merge function to eight upstream publishers.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let a: A

A publisher to merge.

let b: B

A second publisher to merge.

let c: C

A third publisher to merge.

let d: D

A fourth publisher to merge.

let e: E

A fifth publisher to merge.

let f: F

A sixth publisher to merge.

let g: G

An seventh publisher to merge.

let h: H

A eighth publisher to merge.

### Comparing Publishers

static func == (Publishers.Merge8&lt;A, B, C, D, E, F, G, H>, Publishers.Merge8&lt;A, B, C, D, E, F, G, H>) -> Bool

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

struct MergeMany

A publisher created by applying the merge function to an arbitrary number of upstream publishers.

struct Zip

A publisher created by applying the zip function to two upstream publishers.

struct Zip3

A publisher created by applying the zip function to three upstream publishers.

struct Zip4

A publisher created by applying the zip function to four upstream publishers.

