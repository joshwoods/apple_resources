

- UIKit
-  UIInputViewAudioFeedback 

Protocol

# UIInputViewAudioFeedback

A property that enables a custom input or keyboard accessory view to play standard keyboard input clicks.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIInputViewAudioFeedback : NSObjectProtocol
```

## Overview

Implement this protocol in your custom subclass of UIView that you associate with your custom input nib file. For more information, see Text Programming Guide for iOS.

Implementation of this protocol is optional but expected.

## Topics

### Enabling input clicks

var enableInputClicksWhenVisible: Bool

Specifies whether or not an input view enables input clicks.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Custom keyboard

protocol UITextDocumentProxy

An object that provides textual context to a custom keyboard.

class UIInputViewController

The primary view controller for a custom keyboard app extension.

class UILexicon

A read-only array of term pairs, each in a lexicon entry object, for a custom keyboard.

class UILexiconEntry

A read-only term pair, available within a lexicon object, for a custom keyboard.

