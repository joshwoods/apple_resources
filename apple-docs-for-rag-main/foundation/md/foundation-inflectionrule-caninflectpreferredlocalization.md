

- Foundation
- InflectionRule
-  canInflectPreferredLocalization 

Type Property

# canInflectPreferredLocalization

A Boolean value that indicates whether the rule can inflect the user’s current preferred localization.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var canInflectPreferredLocalization: Bool { get }
```

## Discussion

This value doesn’t change throughout the lifetime of a process.

## See Also

### Determining Availability

static func canInflect(language: String) -> Bool

Returns a Boolean value that indicates whether the rule can inflect a given language.

