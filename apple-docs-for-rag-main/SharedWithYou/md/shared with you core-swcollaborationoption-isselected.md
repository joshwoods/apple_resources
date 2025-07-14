

- Shared With You Core
- SWCollaborationOption
-  isSelected 

Instance Property

# isSelected

A Boolean value that represents the selected state of an option.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var isSelected: Bool { get set }
```

## Discussion

For switches, the app can manually set `isSelected`.

## See Also

### Accessing option attributes

var identifier: String

A unique identifier.

var requiredOptionsIdentifiers: [String]

An array of option identifiers that the app must select before the system makes the option interactive.

var subtitle: String

A localized string the system displays to represent the permissions option in the collaboration view.

var title: String

A localized string the system displays as a title to represent the permissions option.

