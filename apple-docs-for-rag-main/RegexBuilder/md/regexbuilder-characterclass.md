

- RegexBuilder
-  CharacterClass 

Structure

# CharacterClass

A class of characters that match in a regex.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct CharacterClass
```

## Overview

A character class can represent individual characters, a group of characters, the set of character that match some set of criteria, or a set algebraic combination of all of the above.

## Topics

### Instance Properties

var inverted: CharacterClass

A character class that matches any character that does not match this character class.

### Instance Methods

func intersection(CharacterClass) -> CharacterClass

Returns a character class from the intersection of this class and the given class.

func subtracting(CharacterClass) -> CharacterClass

Returns a character class by subtracting the given class from this class.

func symmetricDifference(CharacterClass) -> CharacterClass

Returns a character class matching elements in one or the other, but not both, of this class and the given class.

func union(CharacterClass) -> CharacterClass

Returns a character class from the union of this class and the given class.

### Type Methods

static func generalCategory(Unicode.GeneralCategory) -> CharacterClass

Returns a character class that matches any element with the given Unicode general category.

### Default Implementations

RegexComponent Implementations

## Relationships

### Conforms To

- Copyable
- RegexComponent

## See Also

### Components

struct Anchor

A regex component that matches a specific condition at a particular position in an input string.

struct Lookahead

A regex component that allows a match to continue only if its contents match at the given location.

struct NegativeLookahead

A regex component that allows a match to continue only if its contents do not match at the given location.

struct ChoiceOf

A regex component that chooses exactly one of its constituent regex components when matching.

