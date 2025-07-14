

- Messages
-  MSMessagesAppTranscriptPresentation 

Protocol

# MSMessagesAppTranscriptPresentation

A protocol that provides support for displaying live messages in the transcript of the Messages app.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
protocol MSMessagesAppTranscriptPresentation
```

## Overview

These methods are called when a view controller is presented using a MSMessagesAppPresentationStyle.transcript presentation style.

## Topics

### Providing the Content’s Size

func contentSizeThatFits(CGSize) -> CGSize

The size of your messages view, given the provided maximum size.

**Required**

## Relationships

### Conforming Types

- MSMessagesAppViewController

## See Also

### Custom iMessage app interface

IceCreamBuilder: Building an iMessage Extension

Allow users to collaborate on the design of ice cream sundae stickers.

Creating a Sticker App with a Custom Layout

Expand on the Messages sticker app template to create an app with a customized user interface.

class MSMessagesAppViewController

The principal view controller for iMessage apps.

enum MSMessagesAppPresentationStyle

Presentation styles that describe your iMessage app’s appearance.

