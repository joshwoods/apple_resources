

- MusicKit
-  TitledSection 

Structure

# TitledSection

A section you can use to request items from the library grouped by title.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct TitledSection
```

## Overview

For example, when you perform a library sectioned request of albums, the library sectioned response will contain albums grouped by the first letter of their title, and the title property of this section will be equal to that first letter.

## Topics

### Operators

static func == (TitledSection, TitledSection) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

var id: MusicItemID

The unique identifier for the titled section.

let title: String

The title of the section.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Identifiable
- MusicLibrarySectionRequestable
- Sendable

