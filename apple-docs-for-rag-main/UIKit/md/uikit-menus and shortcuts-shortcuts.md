

- UIKit
-  Menus and shortcuts 

API Collection

# Menus and shortcuts

Simplify interactions with your app using menu systems, contextual menus, Home Screen quick actions, and keyboard shortcuts.

## Topics

### Menu elements and keyboard shortcuts

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

Adopting menus and UIActions in your user interface

Add menus to your user interface, with built-in button support and bar-button items, and create custom menu experiences.

class UIMenuElement

An object representing a menu, action, or command.

class UIAction

A menu element that performs its action in a closure.

class UICommand

A menu element that performs its action in a selector.

class UIKeyCommand

An object that specifies a key press perform on a hardware keyboard and the resulting action.

class UIDeferredMenuElement

A placeholder menu element that the system replaces with the result of the block’s completion handler.

struct Attributes

Attributes that determine the style of the menu element.

enum State

Constants that indicate the state of an action- or command-based menu element.

protocol UIMenuLeaf

An interface for an object that represents a menu element without child elements.

### Edit menus

class UIEditMenuInteraction

An interaction that provides edit operations using a menu.

protocol UIEditMenuInteractionDelegate

The methods for customizing the menu the interaction displays.

class UIEditMenuConfiguration

An object containing the configuration details for the menu your app presents in response to an edit menu interaction.

protocol UIResponderStandardEditActions

A set of standard methods that apps can adopt to support editing.

### App menus

class UIMenu

A container for grouping related menu elements in an app menu or contextual menu.

protocol UIMenuBuilder

An interface for adding and removing menus from a menu system.

class UIMenuSystem

An object representing a main or contextual menu system.

### Contextual menus

class UIContextMenuInteraction

An interaction object that you use to display relevant actions for your content.

protocol UIContextMenuInteractionDelegate

The methods for providing the set of actions to perform on your content, and for customizing the preview of that content.

class UITargetedPreview

An object describing the view to use during preview-related animations.

class UIPreviewTarget

An object that specifies the container view to use for animations.

class UIPreviewParameters

Additional parameters to use when animating a preview interface.

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

enum UITextSearchFoundTextStyle

Constants that describe the style a find session uses to decorate the text.

enum WordMatchMethod

Constants that describe the method to use when searching text for words that match a string.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

### Home Screen quick actions

Add Home Screen quick actions

Expose commonly used functionality with static or dynamic 3D Touch Home Screen quick actions.

class UIApplicationShortcutItem

An application shortcut item, also called a Home Screen dynamic quick action, that specifies a user-initiated action for your app.

class UIApplicationShortcutIcon

An image you can optionally associate with a Home Screen quick action to improve its appearance and usability.

class UIMutableApplicationShortcutItem

A mutable Home Screen dynamic quick action, which is an item that specifies a configurable user-initiated action for your app.

## See Also

### User interactions

Touches, presses, and gestures

Encapsulate your app’s event-handling logic in gesture recognizers so that you can reuse that code throughout your app.

Drag and drop

Bring drag and drop to your app by using interaction APIs with your views.

Pointer interactions

Support pointer interactions in your custom controls and views.

Apple Pencil interactions

Handle user interactions like double tap and squeeze on Apple Pencil.

Focus-based navigation

Navigate the interface of your UIKit app using a remote, game controller, or keyboard.

Accessibility for UIKit

Make your UIKit apps accessible to everyone who uses iOS and tvOS.

