

- Foundation
-  NSKeyValueObservingOptions 

Structure

# NSKeyValueObservingOptions

The values that can be returned in a change dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSKeyValueObservingOptions
```

## Overview

These constants are passed to addObserver(_:forKeyPath:options:context:) and determine the values that are returned as part of the change dictionary passed to an observeValue(forKeyPath:of:change:context:). You can pass `0` if you require no change dictionary values.

## Topics

### Constants

static var new: NSKeyValueObservingOptions

Indicates that the change dictionary should provide the new attribute value, if applicable.

static var old: NSKeyValueObservingOptions

Indicates that the change dictionary should contain the old attribute value, if applicable.

static var initial: NSKeyValueObservingOptions

If specified, a notification should be sent to the observer immediately, before the observer registration method even returns.

static var prior: NSKeyValueObservingOptions

Whether separate notifications should be sent to the observer before and after each change, instead of a single notification after the change.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Enumerations

enum NSGrammaticalCase

enum NSGrammaticalDefiniteness

enum NSGrammaticalDetermination

enum NSGrammaticalPerson

enum NSGrammaticalPronounType

enum NSKeyValueChange

The kinds of changes that can be observed.

enum NSKeyValueSetMutationKind

