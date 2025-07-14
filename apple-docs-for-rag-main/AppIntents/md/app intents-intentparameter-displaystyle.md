

- App Intents
- IntentParameter
-  displayStyle 

Instance Property

# displayStyle

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final var displayStyle: IntentParameter.PlacemarkDisplayStyle? { get }
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `CLPlacemark`.

## See Also

### Accessing the display style

enum PlacemarkDisplayStyle

Describes a location’s display style in Shortcuts and Siri Suggestions.

