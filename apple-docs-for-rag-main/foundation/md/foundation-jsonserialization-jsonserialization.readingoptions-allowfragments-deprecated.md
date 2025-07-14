

- Foundation
- JSONSerialization
- JSONSerialization.ReadingOptions
-  allowFragments Deprecated

Type Property

# allowFragments

A deprecated option that specifies that the parser should allow top-level objects that aren’t arrays or dictionaries.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
static var allowFragments: JSONSerialization.ReadingOptions { get }
```

Deprecated

Use fragmentsAllowed instead.

## See Also

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

