

- Foundation
- JSONSerialization
- JSONSerialization.ReadingOptions
-  fragmentsAllowed 

Type Property

# fragmentsAllowed

Specifies that the parser allows top-level objects that aren’t arrays or dictionaries.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var fragmentsAllowed: JSONSerialization.ReadingOptions { get }
```

## See Also

### Reading Options

static var mutableContainers: JSONSerialization.ReadingOptions

Specifies that arrays and dictionaries in the returned object are mutable.

static var mutableLeaves: JSONSerialization.ReadingOptions

Specifies that leaf strings in the JSON object graph are mutable.

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

static var json5Allowed: JSONSerialization.ReadingOptions

Specifies that reading serialized JSON data supports the JSON5 syntax.

static var topLevelDictionaryAssumed: JSONSerialization.ReadingOptions

Specifies that the parser assumes the top level of the JSON data is a dictionary, even if it doesn’t begin and end with curly braces.

static var allowFragments: JSONSerialization.ReadingOptions

A deprecated option that specifies that the parser should allow top-level objects that aren’t arrays or dictionaries.

Deprecated

