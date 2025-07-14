

- Messages
-  MSMessagesAppViewController 

Class

# MSMessagesAppViewController

The principal view controller for iMessage apps.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
class MSMessagesAppViewController
```

## Mentioned in 

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

## Overview

Use this class to manage your extension. For more information on app extensions, see App Extension Programming Guide.

## Topics

### Managing the Extension’s State

var activeConversation: MSConversation?

The conversation currently displayed in the transcript.

func dismiss()

Dismisses the extension and marks it for termination.

func willBecomeActive(with: MSConversation)

Invoked just before the Messages extension becomes active.

func didBecomeActive(with: MSConversation)

Invoked after the Messages extension becomes active.

func willResignActive(with: MSConversation)

Invoked just before the message resigns its active status.

func didResignActive(with: MSConversation)

Invoked after the message resigns its active status.

### Tracking Messages

func willSelect(MSMessage, conversation: MSConversation)

Invoked in response to the user selecting a message object in the transcript, before the system updates the conversation’s selectedMessage property.

func didSelect(MSMessage, conversation: MSConversation)

Invoked in response to the user selecting a message object in the transcript, after the system updates the conversation’s selectedMessage property.

func didReceive(MSMessage, conversation: MSConversation)

Invoked when the iMessage app receives a new message object.

func didStartSending(MSMessage, conversation: MSConversation)

Invoked when the user sends a message object.

func didCancelSending(MSMessage, conversation: MSConversation)

Invoked when the user deletes a message object from the Messages app’s input field.

### Working with Presentation Styles and Contexts

var presentationStyle: MSMessagesAppPresentationStyle

The extension’s current presentation style.

func requestPresentationStyle(MSMessagesAppPresentationStyle)

Asks the extension’s user interface to transition to the provided style.

func willTransition(to: MSMessagesAppPresentationStyle)

Tells the view controller that the extension is about to transition to a new presentation style.

func didTransition(to: MSMessagesAppPresentationStyle)

Tells the view controller that the extension has transitioned to a new presentation style.

enum MSMessagesAppPresentationStyle

Presentation styles that describe your iMessage app’s appearance.

var presentationContext: MSMessagesAppPresentationContext

The context describing where your iMessage app is presented.

enum MSMessagesAppPresentationContext

Presentation contexts describing where your iMessage app appears.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MSMessagesAppTranscriptPresentation
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Custom iMessage app interface

IceCreamBuilder: Building an iMessage Extension

Allow users to collaborate on the design of ice cream sundae stickers.

Creating a Sticker App with a Custom Layout

Expand on the Messages sticker app template to create an app with a customized user interface.

protocol MSMessagesAppTranscriptPresentation

A protocol that provides support for displaying live messages in the transcript of the Messages app.

enum MSMessagesAppPresentationStyle

Presentation styles that describe your iMessage app’s appearance.

