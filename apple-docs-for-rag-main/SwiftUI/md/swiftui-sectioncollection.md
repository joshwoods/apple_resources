

- SwiftUI
-  SectionCollection 

Structure

# SectionCollection

An opaque collection representing the sections of view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct SectionCollection
```

## Overview

Sections are constructed lazily, on demand, so access only as much of this collection as is necessary to create the resulting content.

You can get access to a view’s SectionCollection by using the `Group/init(sectionsOf:transform:)` initializer.

Any content of the given view which is not explicitly specified as a section is grouped with its sibling content to form implicit sections, meaning the minimum number of sections in a `SectionCollection` is one.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- RandomAccessCollection
- Sequence

## See Also

### Organizing views into sections

struct Section

A container view that you can use to add hierarchy within certain views.

struct SectionConfiguration

Specifies the contents of a section.

