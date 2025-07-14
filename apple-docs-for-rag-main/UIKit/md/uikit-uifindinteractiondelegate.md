

- UIKit
-  UIFindInteractionDelegate 

Protocol

# UIFindInteractionDelegate

A delegate object that provides a session object to manage the search state for a find interaction and receives notifications of search session lifetimes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
protocol UIFindInteractionDelegate : NSObjectProtocol
```

## Topics

### Beginning the search

func findInteraction(UIFindInteraction, sessionFor: UIView) -> UIFindSession?

Provides the object for managing the state, presentation, and behavior of the search.

**Required**

### Decorating the searched content

func findInteraction(UIFindInteraction, didBegin: UIFindSession)

Informs the delegate when the interaction is about to present the find panel.

func findInteraction(UIFindInteraction, didEnd: UIFindSession)

Informs the delegate when the interaction is about to dismiss the find panel.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UITextView

## See Also

### Find and replace

class UIFindInteraction

An interaction that provides text finding and replacing operations using a system find panel.

class UIFindSession

An abstract base class that manages the state, presentation, and behavior for a search that the find interaction initiates.

class UITextSearchingFindSession

A find session object that wraps a searchable object implementing the text-searching protocol.

protocol UITextSearching

The methods you use on a find session’s searchable objects to perform search operations and decorate the found text results.

class UITextSearchOptions

An object containing the configurable options for a text search.

enum UITextSearchFoundTextStyle

Constants that describe the style a find session uses to decorate the text.

enum WordMatchMethod

Constants that describe the method to use when searching text for words that match a string.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

