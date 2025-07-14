

- UIKit
-  UIAccessibilityCustomRotor 

Class

# UIAccessibilityCustomRotor

A context-sensitive function that helps VoiceOver users find the next instance of a related element.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class UIAccessibilityCustomRotor
```

## Overview

You might use an instance of this class to find the next link in an article, or the next misspelled word in a document.

Related Sessions from WWDC20

Session 10116: VoiceOver Efficiency with Custom Rotors

## Topics

### Creating a rotor object

init(attributedName: NSAttributedString, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor with the specified name and search block.

init(name: String, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor with the specified name and search block.

init(systemType: UIAccessibilityCustomRotor.SystemRotorType, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor for the specified type of item.

### Navigating to the next item

var itemSearchBlock: UIAccessibilityCustomRotor.Search

The block for retrieving the next or previous rotor.

typealias Search

The block type for retrieving the next or previous rotor.

enum Direction

Constants that indicate the search direction.

### Getting the rotor type

var systemRotorType: UIAccessibilityCustomRotor.SystemRotorType

The type of content that the rotor searches.

enum SystemRotorType

Constants that indicate the type of content that the rotor represents.

### Identifying the rotor

var name: String

The name of the rotor.

var attributedName: NSAttributedString

The name of the rotor as an attributed string.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Navigation

class UIAccessibilityCustomRotorItemResult

A target element that a custom rotor references.

class UIAccessibilityCustomRotorSearchPredicate

The search parameters that help determine the next matching custom rotor item result.

