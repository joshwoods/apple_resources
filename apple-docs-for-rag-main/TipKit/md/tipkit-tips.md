

- TipKit
-  Tips 

Enumeration

# Tips

TipKit namespace.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
enum Tips
```

## Overview

A collection of objects for controlling the display of your tips.

## Topics

### Actions

struct Action

A type that describes a control associated with a tip.

### Events

struct DonationTimeRange

A duration of time for filtering event donations.

struct EmptyDonation

An empty event donation.

### Options

struct IgnoresDisplayFrequency

Controls whether a tip obeys the preconfigured display frequency interval.

struct MaxDisplayCount

Specifies the maximum number of times a tip displays before the system automatically invalidates it.

struct ConfigurationOption

A type that marks an object as a tip configuration.

struct ParameterOption

A type that represents the various customizations that you can make to a tip parameter.

### Builders

struct ActionBuilder

The result builder for generating a tip’s actions.

struct OptionsBuilder

The result builder for generating a tip’s options.

struct RuleBuilder

The result builder for generating a tip’s rules.

### Status

enum Status

A type that describes the current display eligibility status for a tip.

### Validation

enum InvalidationReason

A type that describes why the system permanently invalidated a tip.

### Structures

struct Event

A repeatable user-defined action.

struct GroupBuilder

struct MaxDisplayDuration

Specifies the maximum amount of time a tip is displayed before it is invalidated.

struct Parameter

A type that monitors the state of its wrapped value to reevaluate any dependent tip rules when the value changes.

struct Rule

A condition to meet before displaying a tip.

### Type Methods

static func configure([Tips.ConfigurationOption]) throws

Loads and configures the persistent state of all tips in your app.

static func hideAllTipsForTesting()

Hide all tips regardless of their display rule eligibility for UI testing without tips.

static func hideTipsForTesting([any Tip.Type])

Hide specified tips regardless of their display rule eligibility for UI testing without certain tips.

static func resetDatastore() throws

Resets the tips’ datastore to the initial state for re-testing tip display rules and eligibility.

static func showAllTipsForTesting()

Show all tips regardless of their display rule eligibility or display frequency status for UI testing of tips.

static func showTipsForTesting([any Tip.Type])

Show specified tips regardless of their display rule eligibility or display frequency status for UI testing of certain tips.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable

