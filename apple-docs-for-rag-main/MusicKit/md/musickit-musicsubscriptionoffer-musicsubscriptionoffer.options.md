

- MusicKit
- MusicSubscriptionOffer
-  MusicSubscriptionOffer.Options 

Structure

# MusicSubscriptionOffer.Options

Options for loading subscription offers for Apple Music.

MusicKitSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Options
```

## Topics

### Initializers

init(action: MusicSubscriptionOffer.Action, messageIdentifier: MusicSubscriptionOffer.MessageIdentifier, itemID: MusicItemID?, affiliateToken: String?, campaignToken: String?)

Creates options for a subscription offer sheet with specific values for common properties.

### Instance Properties

var action: MusicSubscriptionOffer.Action

An action for the subscription offers entry point.

var affiliateToken: String?

An affiliate token for the Apple Services affiliate program.

var campaignToken: String?

A campaign token for the Apple Services affiliate program.

var itemID: MusicItemID?

An identifier for the music item the user is trying to access, which requires an active subscription.

var messageIdentifier: MusicSubscriptionOffer.MessageIdentifier

An identifier for selecting the main message that the subscription offer sheet presents to the user.

### Type Properties

static let `default`: MusicSubscriptionOffer.Options

The default set of options for loading subscription offers for Apple Music.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

