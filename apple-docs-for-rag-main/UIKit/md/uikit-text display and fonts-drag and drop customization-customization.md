

- UIKit
- Text display and fonts
-  Drag and drop customization 

API Collection

# Drag and drop customization

Extend the standard drag and drop support for text views to include custom types of content.

## Overview

The UITextField and UITextView classes provide built-in support for dragging and dropping text and images. You can extend this support to your own custom data types by adding a text drag delegate or text drop delegate to your views. Your text drag delegate adopts the UITextDragDelegate protocol and is responsible for providing the items to be dragged. Your text drop delegate adopts the UITextDropDelegate protocol and handles drops containing items with your custom data types.

## Topics

### Text view additions

protocol UITextDragDelegate

The interface for customizing the behavior of a drag activity for a text view.

protocol UITextDropDelegate

The interface for configuring a text view’s drop behavior.

protocol UITextDraggable

The interface that determines if a text view is a drag source.

struct UITextDragOptions

A set of options that determine the behavior of a draggable text view.

protocol UITextDroppable

The interface that determines if a text view is a drop destination.

enum UITextDropEditability

The text-drop editability styles for noneditable text views.

### Drag content

protocol UITextDragRequest

The interface for describing the attributes of a drag activity originating in a text view.

class UITextDragPreviewRenderer

Renders previews of text dragged by the user.

### Drop management

protocol UITextDropRequest

The interface for specifying the attributes of a drop request for a text view.

class UITextDropProposal

A proposed configuration for the behavior of a text drop interaction.

enum Action

The text drop action styles for text views.

enum Performer

The performers that are responsible for handling the drop operation.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

### Pasteboard support

protocol UITextPasteItem

The interface for obtaining information about, and interacting with, a text item for pasting or dropping.

protocol UISearchTextFieldPasteItem

A protocol that supports pasting tokens.

protocol UITextPasteDelegate

The interface for handling pasting and dropping of text, using item providers.

protocol UITextPasteConfigurationSupporting

The interface for text-oriented responder objects to participate in the unified paste and drop system in iOS.

## See Also

### Text views

class UILabel

A view that displays one or more lines of informational text.

class UITextField

An object that displays an editable text area in your interface.

class UITextView

A scrollable, multiline text region.

