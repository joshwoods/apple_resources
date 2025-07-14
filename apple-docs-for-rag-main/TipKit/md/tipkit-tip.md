

- TipKit
-  Tip 

Protocol

# Tip

A type that sets a tip’s content, as well as the conditions for when it displays.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol Tip : Identifiable, Sendable
```

## Overview

Use this protocol for setting a tip’s content, as well as defining the conditions for when it appears in a view. You create custom tips by declaring types that conform to the `Tip` protocol. Set your tip’s content by giving it a title, message, image, and a list of actions.

For example, to create a tip with a `title`, `message`, and `image`:

```
struct FavoriteBackyardTip: Tip {
    var title: Text {
        Text("Save as a Favorite")
    }

    var message: Text? {
        Text("Your favorite backyards always appear at the top of the list.")
    }

    var image: Image? {
        Image(systemName: "star")
    }
}
```

For a tip to be valid, you need to set its `title`. To control when a tip displays, pass instances of Tip.Rule and Tip.Option into the rules and options properties of the tip.

After you define your tip’s content, display it in either a TipView or a popoverTip(_:arrowEdge:action:).

## Topics

### Setting tip content

var title: Text

A title that names the tip.

**Required**

var message: Text?

A short description of how to use the tip’s feature.

**Required**

var image: Image?

The image associated with the tip.

**Required**

var id: String

The tip’s unique identifier.

**Required**

### Controlling when tips appear

var rules: [Self.Rule]

The rules that determine when a tip is eligible for display. For more information on rules, see Tips.Rule.

**Required**

typealias Rule

A condition to meet before displaying a tip.

typealias Event

A repeatable user-defined action.

### Customizing tip behavior

var options: [any TipOption]

Customizations for a tip.

**Required**

typealias Option

A type that represents the various customizations that you can make to a tip’s behavior.

### Providing actions

var actions: [Self.Action]

Buttons that help people get started or learn more about your feature.

**Required**

typealias Action

A type that describes a control associated with a tip.

### Monitoring tip status

var status: Self.Status

The current status of a tip based on its rules and the configured displayFrequency(_:).

var statusUpdates: AsyncStream&lt;Self.Status>

An asynchronous sequence for monitoring a tip’s status changes.

var shouldDisplay: Bool

A Boolean value that determines whether to display a tip.

var shouldDisplayUpdates: AsyncMapSequence&lt;AsyncStream&lt;Self.Status>, Bool>

An asynchronous sequence for monitoring a tip’s display eligibility.

typealias Status

A type that describes the current display eligibility status for a tip.

typealias InvalidationReason

A type that describes why the system permanently invalidated a tip.

### Invalidating a tip

func invalidate(reason: Self.InvalidationReason)

Permanently invalidates a tip and prevents it from displaying.

### Type Aliases

typealias IgnoresDisplayFrequency

Controls whether a tip obeys the preconfigured display frequency interval.

typealias MaxDisplayCount

Specifies the maximum number of times a tip displays before the system automatically invalidates it.

typealias MaxDisplayDuration

Specifies the maximum amount of time a tip is displayed before it is invalidated.

## Relationships

### Inherits From

- Identifiable
- Sendable

### Conforming Types

- AnyTip

## See Also

### Content

class TipGroup

A collection of tips that can be presented one at a time using a specific order or based on the first tip eligible for display.

