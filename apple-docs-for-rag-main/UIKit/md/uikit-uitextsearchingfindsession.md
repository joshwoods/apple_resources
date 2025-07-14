

- UIKit
-  UITextSearchingFindSession 

Class

# UITextSearchingFindSession

A find session object that wraps a searchable object implementing the text-searching protocol.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class UITextSearchingFindSession
```

## Overview

Implement the UITextSearching protocol on the class that encapsulates the searchable content for your view to use an instance of UITextSearchingFindSession as the session object. Alternatively, you can subclass UIFindSession to manage the details of the session using a custom class.

The find session’s reference to searchableObject is weakly held to avoid a retain cycle if the view you install the interaction on is the searchable object itself. Ensure that your app maintains a strong reference to the searchable object.

## Topics

### Creating a text searching find session

init(searchableObject: any __UITextSearching)

Initializes an object to manage the search for the searchable object you specify.

convenience init&lt;SearchableObject>(searchableObject: SearchableObject)

Initializes an object to manage the search for the searchable object you specify.

### Getting the searchable object

var searchableObject: (any __UITextSearching)?

The object to search, responsible for performing the search operation and decorating the results.

## Relationships

### Inherits From

- UIFindSession

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Find and replace

class UIFindInteraction

An interaction that provides text finding and replacing operations using a system find panel.

protocol UIFindInteractionDelegate

A delegate object that provides a session object to manage the search state for a find interaction and receives notifications of search session lifetimes.

class UIFindSession

An abstract base class that manages the state, presentation, and behavior for a search that the find interaction initiates.

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

