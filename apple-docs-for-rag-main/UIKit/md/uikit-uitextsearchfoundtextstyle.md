

- UIKit
-  UITextSearchFoundTextStyle 

Enumeration

# UITextSearchFoundTextStyle

Constants that describe the style a find session uses to decorate the text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum UITextSearchFoundTextStyle
```

## Overview

Use UITextSearchFoundTextStyle to identify ranges of text your app decorates to indicate matches, highlighted matches and non-matching text.

## Topics

### Constants

case normal

A style that indicates the text isn’t a match.

case found

A style that indicates the text is a match, but not highlighted.

case highlighted

A style that indicates the text is a highlighted match.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Find and replace

class UIFindInteraction

An interaction that provides text finding and replacing operations using a system find panel.

protocol UIFindInteractionDelegate

A delegate object that provides a session object to manage the search state for a find interaction and receives notifications of search session lifetimes.

class UIFindSession

An abstract base class that manages the state, presentation, and behavior for a search that the find interaction initiates.

class UITextSearchingFindSession

A find session object that wraps a searchable object implementing the text-searching protocol.

protocol UITextSearching

The methods you use on a find session’s searchable objects to perform search operations and decorate the found text results.

class UITextSearchOptions

An object containing the configurable options for a text search.

enum WordMatchMethod

Constants that describe the method to use when searching text for words that match a string.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

