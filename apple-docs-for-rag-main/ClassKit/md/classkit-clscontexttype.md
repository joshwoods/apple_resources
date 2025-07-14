

- ClassKit
-  CLSContextType 

Enumeration

# CLSContextType

The kinds of assignable content a context can contain.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
enum CLSContextType
```

## Overview

When you initialize a new context with init(type:identifier:title:), you specify its type to provide an indication of how your content is structured. The type doesn’t affect the context’s behavior, but it does provide an important indicator to teachers trying to understand your app’s content.

## Topics

### Context Types

case app

An app context.

case audio

An audio context.

case book

A book context.

case challenge

A challenge context.

case chapter

A chapter context.

case course

A context that represents an entire course.

case custom

A context for assignable content that isn’t represented by one of the built-in context types.

case document

A document context.

case exercise

An exercise context.

case game

A game context.

case lesson

A lesson context.

case level

A level context.

case none

No type is assigned.

case page

A page context.

case quiz

A quiz context.

case section

A section context.

case task

A task context.

case video

A video context.

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

### Managing the context type

var type: CLSContextType

The kind of content a context represents.

func setType(CLSContextType)

Updates the kind of content that a context represents.

var customTypeName: String?

An optional name that the system presents to the user if you choose the custom context type.

