

- StoreKit
- SubscriptionStoreControlStyleConfiguration
-  SubscriptionStoreControlStyleConfiguration.Section 

Structure

# SubscriptionStoreControlStyleConfiguration.Section

The properties of a section of subscription options within a subscription store control.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Section
```

## Overview

Each value represents an instance of SubscriptionOptionSection when the system creates a SubscriptionStoreView.

Even if a subscription store instance doesn’t declare sections using SubscriptionOptionSection, the instance always has at least one implicit section that contains the options within the group. Implicit sections have `nil` for the header and footer accessory views.

## Topics

### Getting a section’s content

var options: [SubscriptionStoreControlStyleConfiguration.Option]

The subscription options to merchandise within a section.

### Getting accessory views

var header: SubscriptionStoreControlStyleConfiguration.Section.Header?

A decorative header view for a section that displays before the options.

var footer: SubscriptionStoreControlStyleConfiguration.Section.Footer?

A decorative footer view for a section that displays after the options.

struct Header

A type-erased header of a section of subscription options.

struct Footer

A type-erased footer of a section of subscription options.

### Identifying a section

struct ID

The stable identity of a section of subscription options.

## Relationships

### Conforms To

- Identifiable

## See Also

### Getting subscription options to merchandise

var options: [SubscriptionStoreControlStyleConfiguration.Option]

An array of subscription options for the subscription store view to merchandise.

var sections: [SubscriptionStoreControlStyleConfiguration.Section]

The subscription options to merchandise by sections.

struct Option

Properties of an auto-renewable subscription option to merchandise.

struct PickerOption

The properties of a picker option to use for selecting a subscription.

struct Icon

A type-erased icon of a subscription option.

