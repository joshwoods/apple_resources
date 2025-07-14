

- Core Spotlight
- CSSearchableItem
-  CSSearchableItem.UpdateListenerOptions 

Structure

# CSSearchableItem.UpdateListenerOptions

The set of options that contain metadata-associated summarization and prioritization of a searchable item.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct UpdateListenerOptions
```

## Discussion

To receive updates to specific properties on searchable items, implement the searchableItemsDidUpdate(_:) delegate method.

## Topics

### Initializers

init(rawValue: UInt)

An unsigned integer that describes the listener options.

### Type Properties

static var priority: CSSearchableItem.UpdateListenerOptions

A value that describes the listener priority options.

static var summarization: CSSearchableItem.UpdateListenerOptions

A value that describes the listener summarization options.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

