

- SwiftUI
-  SubviewsCollection 

Structure

# SubviewsCollection

An opaque collection representing the subviews of view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct SubviewsCollection
```

## Overview

Subviews collection constructs subviews on demand, so only access the part of the collection you need to create the resulting content.

You can get access to a view’s subview collection by using the `Group/init(sectionsOf:transform:)` initializer.

The collection’s elements are the pieces that make up the given view, and the collection as a whole acts as a proxy for the original view.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- RandomAccessCollection
- Sequence
- View

## See Also

### Accessing a container’s subviews

struct Subview

An opaque value representing a subview of another view.

struct SubviewsCollectionSlice

func containerValue&lt;V>(WritableKeyPath&lt;ContainerValues, V>, V) -> some View

Sets a particular container value of a view.

struct ContainerValues

A collection of container values associated with a given view.

protocol ContainerValueKey

A key for accessing container values.

