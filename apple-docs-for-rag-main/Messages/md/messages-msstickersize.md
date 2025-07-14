

- Messages
-  MSStickerSize 

Enumeration

# MSStickerSize

The size of the stickers in the browser view.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
enum MSStickerSize
```

## Overview

The browser scales down sticker images to fit. If a sticker is smaller than the provided space, the browser centers the sticker in the space.

## Topics

### Constants

case small

Small stickers.

case regular

Medium-sized stickers.

case large

Large stickers.

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

### Custom sticker packs

Adding Sticker packs and iMessage apps to the system Stickers app, Messages camera, and FaceTime

Enable your Sticker pack or iMessage app in the media context.

Adding your sticker packs to Messages

Drag and drop your sticker pack into the Stickers asset catalog to let people access your stickers from Messages.

class MSStickerBrowserViewController

A view controller that provides dynamic content to the standard sticker browser.

class MSStickerBrowserView

A browser view that displays a dynamically generated list of stickers.

class MSStickerView

A view for displaying a sticker.

