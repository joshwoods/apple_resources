

- UIKit
-  UIFindInteraction 

Class

# UIFindInteraction

An interaction that provides text finding and replacing operations using a system find panel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class UIFindInteraction
```

## Mentioned in 

Building a desktop-class iPad app

## Overview

Use a find interaction to add text-finding capabilities to your view.

When invoking the interaction, the system displays a find panel for entering a string to search, with buttons for navigating between results. When supporting replacement, this also includes a field for the text replacing matches. The find panel presents as a part of the onscreen keyboard when visible, or inline as part of the receiver’s view hierarchy.

Input from a hardware keyboard triggers a find interaction using standard system shortcuts such as Command+F for find, Command+G for find next, and Command+Shift+G for find previous. Adding the interaction also enables these commands in the menu bar on macOS when your view becomes first responder. You can also trigger the interaction by calling the presentFindNavigator(showingReplace:) method on the interaction object, providing access to find and replace operations programatically.

Some classes, such as UITextView, WKWebView, and PDFView, support built-in find interactions. To enable the interaction on these views, set isFindInteractionEnabled to `true`.

```
textView.isFindInteractionEnabled = true
```

To add find and replace operations to other views:

1.  Create the find interaction object, passing a delegate into the default initializer.

2.  Add the interaction by calling the addInteraction(_:) method on the view.

3.  Provide a UIFindSession object to manage the search performed on the content displayed in the view. You return this object through the findInteraction(_:sessionFor:) method on the delegate.

The following example creates a find interaction for a view that presents searchable content for a document.

```
let document = Document(string: "")
lazy var interactionView = InteractionView(document: document)

lazy var findInteraction = UIFindInteraction(sessionDelegate: self)

override func viewDidLoad() {
    super.viewDidLoad()

    // Add the find interaction.
    interactionView.addInteraction(findInteraction)
}

func findInteraction(_ interaction: UIFindInteraction, sessionFor view: UIView) -> UIFindSession? {
    // Return a searchable object.
    return UITextSearchingFindSession(searchableObject: document)
}
```

Implement the UITextSearching protocol on the class that encapsulates the searchable content for your view to use an instance of UITextSearchingFindSession as the session object. Alternatively, you can subclass UIFindSession when you want to manage the details of the session using a custom class.

Related Sessions from WWDC22

Session 10071: Adopt desktop-class editing interactions

## Topics

### Creating a find interaction

init(sessionDelegate: any UIFindInteractionDelegate)

Initializes a find interaction object with the delegate object you specify.

### Managing find interactions

var delegate: (any UIFindInteractionDelegate)?

An object that updates your app’s presentation and provides the session object for managing the interaction’s search.

func presentFindNavigator(showingReplace: Bool)

Begins a search, displaying the find panel.

func dismissFindNavigator()

Dismisses the find panel, if present.

func findNext()

Highlights the next found result in the content, relative to the currently highlighted result.

func findPrevious()

Highlights the previously found result in the document, relative to the currently highlighted result.

### Configuring the find panel

var isFindNavigatorVisible: Bool

A Boolean value that indicates when the find panel displays onscreen.

var searchText: String?

The search query with which to prepopulate the find panel’s search text field.

var replacementText: String?

The replacement string with which to prepopulate the find panel’s replace text field.

var optionsMenuProvider: (([UIMenuElement]) -> UIMenu?)?

A closure that populates the search options for a find interaction.

### Managing the search

var activeFindSession: UIFindSession?

The object that manages the state, presentation, and behavior of an active search.

func updateResultCount()

Updates the results the interface displays for the active search.

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
- UIInteraction

## See Also

### Related Documentation

Building a desktop-class iPad app

Optimize your iPad app’s user experience by adopting desktop-class enhancements for multitasking with Stage Manager, document interactions, text editing, search, and more.

### Find and replace

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

enum UITextSearchFoundTextStyle

Constants that describe the style a find session uses to decorate the text.

enum WordMatchMethod

Constants that describe the method to use when searching text for words that match a string.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

