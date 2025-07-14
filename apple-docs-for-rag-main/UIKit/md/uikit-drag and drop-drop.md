

- UIKit
-  Drag and drop 

API Collection

# Drag and drop

Bring drag and drop to your app by using interaction APIs with your views.

iOS 11.0+iPadOS 11.0+

## Overview

With drag and drop in iOS, users can drag items from one onscreen location to another using continuous gestures. A drag-and-drop activity can take place in a single app, or it can start in one app and end in another.

Note

Prior to iOS 15, drag-and-drop activities on iPhone can take place in a single app but not between two apps.

The app from which an item is dragged is the *source app*. The app on which an item is dropped is the *destination app*. For drag and drop in a single app, that app plays both roles simultaneously. The complete user action from start to finish — using system-mediated gestures — is a *drag activity*. A *drag session*, by contrast, is an object that’s managed by the system and that manages the items the user is dragging.

When dragging is in progress, the source and destination apps continue to run normally and support user interaction. A user can invoke the Dock, return to the Home screen, open a second app in Split View, and even start another drag activity.

Unlike in macOS, iOS drag and drop supports multiple simultaneous drag activities—as many as the user’s fingers can handle. You can design your app so that the user can sequentially add drag items to an in-progress drag session, and a destination app can accept multiple, simultaneous drops.

Text views and text fields automatically support drag and drop. Collection views and table views offer dedicated, view-specific methods and properties, and text views offer APIs for customizing the views’ drag-and-drop behavior. You can configure any custom view to support drag and drop, as well.

Note

The system handles all security aspects of inter-app drag and drop in iOS. You don’t need to perform additional configuration like setting special entitlements or `Info.plist` keys.

## Topics

### Essentials

Understanding a drag item as a promise

Use drag items to convey data representation promises between a source app and a destination app.

Making a view into a drag source

Adopt drag interaction APIs to provide items for dragging.

Making a view into a drop destination

Adopt drop interaction APIs to selectively consume dragged content.

Adopting drag and drop in a custom view

Demonstrates how to enable drag and drop for a `UIImageView` instance.

Adopting drag and drop in a table view

Demonstrates how to enable and implement drag and drop for a table view.

### Drag and drop interactions

Add interactions to your views to make them drag sources or drop destinations.

protocol UIDragInteractionDelegate

The interface for configuring and controlling a drag interaction.

protocol UIDropInteractionDelegate

The interface for configuring and controlling a drop interaction.

class UIDragInteraction

An interaction to enable dragging of items from a view, employing a delegate to provide drag items and to respond to calls from the drag session.

class UIDropInteraction

An interaction to enable dropping of items onto a view, employing a delegate to instantiate objects and respond to calls from the drop session.

### Spring-loaded interactions

Enable spring loading to support drag and drop for your navigable UI.

protocol UISpringLoadedInteractionBehavior

The interface for specifying the behavior of a spring-loaded interaction.

protocol UISpringLoadedInteractionSupporting

The interface that determines if an object supports a spring-loaded interaction for drag and drop activities.

class UISpringLoadedInteraction

An interaction object for configuring and controlling spring-loaded, user-driven navigation during a drag activity.

protocol UISpringLoadedInteractionContext

The interface an object implements to provide information about a spring-loaded interaction.

protocol UISpringLoadedInteractionEffect

The interface for providing visual styling to a spring-loaded interaction based on the interaction state.

### Drag sources

Specify drag items for drag and drop.

class UIDragItem

A representation of an underlying data item as a person drags it from one location to another.

protocol UIDragDropSession

The common interface for querying the state of both drag sessions and drop sessions.

protocol UIDragSession

The interface for configuring a drag session.

protocol UIDragAnimating

The interface for providing custom animation alongside the system’s lift, drop, and cancellation animations.

### Drop destinations

Specify how a destination view consumes drag items.

protocol UIDropSession

The interface for querying a drop session about its state and associated drag items.

class UIDropProposal

A configuration for the behavior of a drop interaction, required if a view accepts drop activities.

enum UIDropOperation

Operation types that determine how a drag and drop activity resolves when the user drops a drag item.

enum UIDropSessionProgressIndicatorStyle

The drop-progress indicator styles for the drop session, used while data is moving from the source to the destination.

### Item providers

Work with data-representation promises for drag and drop.

Data delivery with drag and drop

Share data between iPad apps during a drag and drop operation using an item provider.

class NSItemProvider

An item provider for conveying data or a file between processes during drag-and-drop or copy-and-paste activities, or from a host app to an app extension.

protocol NSItemProviderReading : NSObjectProtocol

The protocol for implementing a class to allow an item provider to create an instance of the class.

protocol NSItemProviderWriting : NSObjectProtocol

The protocol for implementing a class to allow an item provider to retrieve data from an instance of the class.

protocol UIItemProviderPresentationSizeProviding

protocol UIItemProviderReadingAugmentationDesignating

protocol UIItemProviderReadingAugmentationProviding

### Pasteboard support

Simplify the requesting and consuming of appropriate data representations for pasted and dropped items.

class UIPasteConfiguration

The interface that an object implements to declare its ability to accept specific data types for pasting and for drag-and-drop activities.

protocol UIPasteConfigurationSupporting

The interface that determines whether a responder object supports paste configuration.

### Custom drag item previews

Apply customizations to make drag item previews more appealing and meaningful to the user.

class UIDragPreviewParameters

A set of parameters for adjusting the appearance of a drag item preview or a targeted drag item preview.

class UIDragPreview

A graphical preview for a single drag item, used by the system after a drag has started and when no related animation is running.

class UIDragPreviewTarget

A geometric specification for the source or destination of a drag item preview, used by the system when a user drops items or cancels a drag activity.

class UITargetedDragPreview

A drag item preview used by the system during lift, drop, or cancellation animation.

## See Also

### User interactions

Touches, presses, and gestures

Encapsulate your app’s event-handling logic in gesture recognizers so that you can reuse that code throughout your app.

Menus and shortcuts

Simplify interactions with your app using menu systems, contextual menus, Home Screen quick actions, and keyboard shortcuts.

Pointer interactions

Support pointer interactions in your custom controls and views.

Apple Pencil interactions

Handle user interactions like double tap and squeeze on Apple Pencil.

Focus-based navigation

Navigate the interface of your UIKit app using a remote, game controller, or keyboard.

Accessibility for UIKit

Make your UIKit apps accessible to everyone who uses iOS and tvOS.

