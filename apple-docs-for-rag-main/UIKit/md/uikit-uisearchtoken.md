

- UIKit
-  UISearchToken 

Class

# UISearchToken

Search criteria in a search text field, represented by text and an optional icon.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UISearchToken
```

## Overview

Use search tokens to help users understand and edit complex search queries in a UISearchTextField. A token acts like a single character in standard text interactions such as deleting, selecting, or dragging. A search token should always have text and may also have an icon.

Assign a representedObject to each search token that’s meaningful to your app. By attaching this extra data to the token you can reconstruct the full search query using information available in the search field when, for example, your app starts from state restoration or the user starts a search.

See Using suggested searches with a search controller to learn how to use search tokens.

## Topics

### Creating a search token

init(icon: UIImage?, text: String)

Creates a search token with the specified text and icon (if any).

var representedObject: Any?

The object represented by the search token.

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

### Search field

class UISearchTextField

A view for displaying and editing text and search tokens.

protocol UISearchTextFieldDelegate

The interface for the delegate of a search field.

