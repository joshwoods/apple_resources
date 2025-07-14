

- Foundation
-  AttributedStringProtocol 

Protocol

# AttributedStringProtocol

A protocol that provides common functionality to attributed strings and attributed substrings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup
protocol AttributedStringProtocol : AttributedStringAttributeMutation, CustomStringConvertible, Hashable, Sendable
```

## Overview

Don’t declare new conformances to AttributedStringProtocol. Only the AttributedString and AttributedSubstring types in the standard library are valid conforming types.

## Topics

### Applying Attributes

func settingAttributes(AttributeContainer) -> AttributedString

Returns an attributed string by setting the attributed string’s attributes to those in a specified attribute container.

func mergingAttributes(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy) -> AttributedString

Returns an attributed string by merging the attributed string’s attributes with those in a specified attribute container.

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

func replacingAttributes(AttributeContainer, with: AttributeContainer) -> AttributedString

Returns an attributed string by replacing occurrences of attributes in one attribute container with those in another attribute container.

### Searching for a Substring

func range&lt;T>(of: T, options: String.CompareOptions, locale: Locale?) -> Range&lt;AttributedString.Index>?

Returns the range of a substring in the attributed string, if it exists.

### Accessing a Range

subscript&lt;R>(R) -> AttributedSubstring

Returns a substring of the attributed string using a range to indicate the substring bounds.

**Required**

### Accessing Indices

var startIndex: AttributedString.Index

The position of the first character in a nonempty attributed string.

**Required**

var endIndex: AttributedString.Index

A string’s past-the-end position — the position one greater than the last valid subscript argument.

**Required**

func index(AttributedString.Index, offsetByCharacters: Int) -> AttributedString.Index

Returns the position of the character offset a given distance, measured in characters, from a given string index.

func index(AttributedString.Index, offsetByRuns: Int) -> AttributedString.Index

Returns the position of the run offset a given number of runs from a given string index.

func index(AttributedString.Index, offsetByUnicodeScalars: Int) -> AttributedString.Index

Returns the position of the Unicode scalar offset a given distance, measured in Unicode scalars, from a given string index.

func index(afterCharacter: AttributedString.Index) -> AttributedString.Index

Returns the position of the character immediately after another charcter indicated by an index.

func index(afterRun: AttributedString.Index) -> AttributedString.Index

Returns the position of the run immediately after a run indicated by an index.

func index(afterUnicodeScalar: AttributedString.Index) -> AttributedString.Index

Returns the position of the Unicode scalar immediately after a Unicode scalar indicated by an index.

func index(beforeCharacter: AttributedString.Index) -> AttributedString.Index

Returns the position of the character immediately before another charcter indicated by an index.

func index(beforeRun: AttributedString.Index) -> AttributedString.Index

Returns the position of the run immediately before a run indicated by an index.

func index(beforeUnicodeScalar: AttributedString.Index) -> AttributedString.Index

Returns the position of the Unicode scalar immediately before a Unicode scalar indicated by an index.

struct Index

A type that represents the position of a character or code unit within an attributed string.

### Accessing Views into the Attributed String

var characters: AttributedString.CharacterView

The characters of the attributed string, as a view into the underlying string.

**Required**

var unicodeScalars: AttributedString.UnicodeScalarView

The Unicode scalars of the attributed string, as a view into the underlying string.

**Required**

var runs: AttributedString.Runs

The attributed runs of the attributed string, as a view into the underlying string.

**Required**

### Accessing Whole-String Attributes

subscript&lt;K>(K.Type) -> K.Value?

Returns an attribute value that corresponds to an attributed string key.

**Required**

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> K.Value?

Returns an attribute value that a key path indicates.

**Required**

enum AttributeDynamicLookup

A type to support dynamic member lookup of attributes and containers.

subscript&lt;S>(dynamicMember _: KeyPath&lt;AttributeScopes, S.Type>) -> ScopedAttributeContainer&lt;S>

Returns a scoped attribute container that a key path indicates.

**Required**

struct ScopedAttributeContainer

An attribute container that allows dynamic member lookup of its contents within the specified attribute scope.

### Comparing Attributed Strings or Substrings

static func == &lt;RHS>(Self, RHS) -> Bool

### Default Implementations

CustomStringConvertible Implementations

Hashable Implementations

## Relationships

### Inherits From

- AttributedStringAttributeMutation
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

### Conforming Types

- AttributedString
- AttributedSubstring

