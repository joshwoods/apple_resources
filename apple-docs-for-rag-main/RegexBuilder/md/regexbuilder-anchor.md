

- RegexBuilder
-  Anchor 

Structure

# Anchor

A regex component that matches a specific condition at a particular position in an input string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct Anchor
```

## Overview

You can use anchors to guarantee that a match only occurs at certain points in an input string, such as at the beginning of the string or at the end of a line.

## Topics

### Instance Properties

var inverted: Anchor

The inverse of this anchor, which matches at every position that this anchor does not.

### Type Properties

static var endOfLine: Anchor

An anchor that matches at the end of a line, including at the end of the input string.

static var endOfSubject: Anchor

An anchor that matches at the end of the input string.

static var endOfSubjectBeforeNewline: Anchor

An anchor that matches at the end of the input string or at the end of the line immediately before the end of the string.

static var firstMatchingPositionInSubject: Anchor

An anchor that matches at the first position of a match in the input string.

static var startOfLine: Anchor

An anchor that matches at the start of a line, including the start of the input string.

static var startOfSubject: Anchor

An anchor that matches at the start of the input string.

static var textSegmentBoundary: Anchor

An anchor that matches at a grapheme cluster boundary.

static var wordBoundary: Anchor

An anchor that matches at a word boundary.

### Default Implementations

RegexComponent Implementations

## Relationships

### Conforms To

- Copyable
- RegexComponent

## See Also

### Components

struct CharacterClass

A class of characters that match in a regex.

struct Lookahead

A regex component that allows a match to continue only if its contents match at the given location.

struct NegativeLookahead

A regex component that allows a match to continue only if its contents do not match at the given location.

struct ChoiceOf

A regex component that chooses exactly one of its constituent regex components when matching.

