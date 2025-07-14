

- Foundation
- JSONSerialization
-  JSONSerialization.ReadingOptions 

Structure

# JSONSerialization.ReadingOptions

Options used when creating Foundation objects from JSON data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct ReadingOptions
```

## Overview

Use these options when parsing JSON with jsonObject(with:options:) and jsonObject(with:options:).

## Topics

### Creating a Reading Options Instance

init(rawValue: UInt)

### Reading Options

static var mutableContainers: JSONSerialization.ReadingOptions

Specifies that arrays and dictionaries in the returned object are mutable.

static var mutableLeaves: JSONSerialization.ReadingOptions

Specifies that leaf strings in the JSON object graph are mutable.

static var fragmentsAllowed: JSONSerialization.ReadingOptions

Specifies that the parser allows top-level objects that aren’t arrays or dictionaries.

static var json5Allowed: JSONSerialization.ReadingOptions

Specifies that reading serialized JSON data supports the JSON5 syntax.

static var topLevelDictionaryAssumed: JSONSerialization.ReadingOptions

Specifies that the parser assumes the top level of the JSON data is a dictionary, even if it doesn’t begin and end with curly braces.

static var allowFragments: JSONSerialization.ReadingOptions

A deprecated option that specifies that the parser should allow top-level objects that aren’t arrays or dictionaries.

Deprecated

static var mutableContainers: JSONSerialization.ReadingOptions

Specifies that arrays and dictionaries in the returned object are mutable.

static var mutableLeaves: JSONSerialization.ReadingOptions

Specifies that leaf strings in the JSON object graph are mutable.

static var fragmentsAllowed: JSONSerialization.ReadingOptions

Specifies that the parser allows top-level objects that aren’t arrays or dictionaries.

static var json5Allowed: JSONSerialization.ReadingOptions

Specifies that reading serialized JSON data supports the JSON5 syntax.

static var topLevelDictionaryAssumed: JSONSerialization.ReadingOptions

Specifies that the parser assumes the top level of the JSON data is a dictionary, even if it doesn’t begin and end with curly braces.

static var allowFragments: JSONSerialization.ReadingOptions

A deprecated option that specifies that the parser should allow top-level objects that aren’t arrays or dictionaries.

Deprecated

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

### Creating a JSON Object

class func jsonObject(with: Data, options: JSONSerialization.ReadingOptions) throws -> Any

Returns a Foundation object from given JSON data.

class func jsonObject(with: InputStream, options: JSONSerialization.ReadingOptions) throws -> Any

Returns a Foundation object from JSON data in a given stream.

