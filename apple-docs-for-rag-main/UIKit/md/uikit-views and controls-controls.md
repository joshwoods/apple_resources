

- UIKit
-  Views and controls 

API Collection

# Views and controls

Present your content onscreen and define the interactions allowed with that content.

## Overview

Views and controls are the visual building blocks of your app’s user interface. Use them to draw and organize your app’s content onscreen.

Views can host other views. Embedding one view inside another creates a containment relationship between the host view (known as the *superview*) and the embedded view (known as the *subview*). View hierarchies make it easier to manage views.

You can also use views to do any of the following:

- Respond to touches and other events (either directly or in coordination with gesture recognizers).

- Draw custom content using Core Graphics or UIKit classes.

- Support drag and drop interactions.

- Respond to focus changes.

- Animate the size, position, and appearance attributes of the view.

UIView is the root class for all views and defines their common behavior. UIControl defines additional behaviors that are specific to buttons, switches, and other views designed for user interactions.

For additional information about how to use views and controls, see Human Interface Guidelines. To see examples of UIKit controls, see UIKit Catalog: Creating and customizing views and controls.

## Topics

### View fundamentals

class UIView

An object that manages the content for a rectangular area on the screen.

UIKit Catalog: Creating and customizing views and controls

Customize your app’s user interface with views and controls.

### Container views

Organize and present large data sets using container views.

Autosizing Views for Localization in iOS

Add auto layout constraints to your app to achieve localizable views.

Collection views

Display nested views using a configurable and highly customizable layout.

Table views

Display data in a single column of customizable rows.

class UIStackView

A streamlined interface for laying out a collection of views in either a column or a row.

class UIScrollView

A view that allows the scrolling and zooming of its contained views.

### Content views

class UIActivityIndicatorView

A view that shows that a task is in progress.

class UICalendarView

A view that displays a calendar with date-specific decorations, and provides for user selection of a single date or multiple dates.

class UIContentUnavailableView

A view that indicates there’s no content to display.

class UIImageView

A view that displays a single image or a sequence of animated images in your interface.

class UIPickerView

A view that uses a spinning-wheel or slot-machine metaphor to show one or more sets of values.

class UIProgressView

A view that depicts the progress of a task over time.

class UIWebView

A view that embeds web content in your app.

Deprecated

### Controls

Gather input and respond to user interactions with controls.

Responding to control-based events using target-action

Handle user input by connecting buttons, sliders, and other controls to your app’s code using the target-action design pattern.

class UIControl

The base class for controls, which are visual elements that convey a specific action or intention in response to user interactions.

class UIButton

A control that executes your custom code in response to user interactions.

class UIColorWell

A control that displays a color picker.

class UIDatePicker

A control for inputting date and time values.

class UIPageControl

A control that displays a horizontal series of dots, each of which corresponds to a page in the app’s document or other data-model entity.

class UISegmentedControl

A horizontal control that consists of multiple segments, each segment functioning as a discrete button.

class UISlider

A control for selecting a single value from a continuous range of values.

class UIStepper

A control for incrementing or decrementing a value.

class UISwitch

A control that offers a binary choice, such as on/off.

### Text views

Display and edit text using text views.

class UILabel

A view that displays one or more lines of informational text.

class UITextField

An object that displays an editable text area in your interface.

class UITextView

A scrollable, multiline text region.

Drag and drop customization

Extend the standard drag and drop support for text views to include custom types of content.

### Search field

class UISearchTextField

A view for displaying and editing text and search tokens.

class UISearchToken

Search criteria in a search text field, represented by text and an optional icon.

protocol UISearchTextFieldDelegate

The interface for the delegate of a search field.

### Visual effects

class UIVisualEffect

An initializer for visual effect views and blur and vibrancy effect objects.

class UIVisualEffectView

An object that implements some complex visual effects.

class UIVibrancyEffect

An object that amplifies and adjusts the color of the content layered behind a visual effect view.

class UIBlurEffect

An object that applies a blurring effect to the content layered behind a visual effect view.

### Bars

Manage the items displayed on navigation bars, tab bars, search bars, and toolbars.

class UIBarItem

An abstract superclass for items that you can add to a bar that appears at the bottom of the screen.

class UIBarButtonItem

A specialized button for placement on a toolbar, navigation bar, or shortcuts bar.

class UIBarButtonItemGroup

A group of one or more bar button items for placement on a navigation bar or shortcuts bar.

class UINavigationBar

Navigational controls that display in a bar along the top of the screen, usually in conjunction with a navigation controller.

class UISearchBar

A specialized view for receiving search-related information from the user.

class UIToolbar

A control that displays one or more buttons along the bottom edge of your interface.

class UITabBar

A control that displays one or more buttons in a tab bar for selecting between different subtasks, views, or modes in an app.

class UITabBarItem

An object that describes an item in a tab bar.

protocol UIBarPositioning

A set of methods for defining the positioning of bars in iOS apps.

protocol UIBarPositioningDelegate

A set of methods that support the positioning of a bar that conforms to the UIBarPositioning protocol.

### Content viewer

class UILargeContentViewerInteraction

An interaction that enables a gesture to present the large content viewer for cases when supporting the largest dynamic type sizes isn’t appropriate.

protocol UILargeContentViewerInteractionDelegate

An object that customizes the behavior of the large content viewer interactions.

protocol UILargeContentViewerItem

Methods that provide details about how to display your custom content in the large content viewer.

### Private Click Measurement (PCM)

class UIEventAttributionView

An overlay view that verifies user interaction for Web AdAttributionKit.

class UIEventAttribution

An object that contains event attribution information for Web AdAttributionKit.

NSAdvertisingAttributionReportEndpoint

The URL where Private Click Measurement and SKAdNetwork send attribution information.

### SwiftUI

Using SwiftUI with UIKit

Learn how to incorporate SwiftUI views into a UIKit app.

### Related types

struct UIOffset

A structure that specifies an amount to offset a position.

struct UIAxis

A structure that specifies the layout axes.

struct UIEdgeInsets

The inset distances for views.

struct NSDirectionalEdgeInsets

The inset distances for views, taking the user interface layout direction into account.

struct NSDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

enum NSRectAlignment

Constants that specify alignment to an edge or a set of edges depending on the user interface layout direction.

struct UIDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

Deprecated

UIKit macros

Macros that UIKit defines.

## See Also

### User interface

View controllers

Manage your interface using view controllers and facilitate navigation around your app’s content.

View layout

Use stack views to lay out the views of your interface automatically. Use Auto Layout when you require precise placement of your views.

Appearance customization

Add Dark Mode support to your app, customize the appearance of bars, and use appearance proxies to modify your UI.

Animation and haptics

Provide feedback to users using view-based animations and haptics.

Windows and screens

Provide a container for your view hierarchies and other content.

