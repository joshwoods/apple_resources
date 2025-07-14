

- CarPlay
-  CPBarButtonProviding 

Protocol

# CPBarButtonProviding

The methods that templates use to provide buttons for the navigation bar.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
protocol CPBarButtonProviding : NSObjectProtocol
```

## Overview

`CPBarButtonProviding` is a protocol that templates use to provide a Back button and leading and trailing buttons for the navigation bar.

You don’t adopt this protocol in your own types. If you want to add buttons to the navigation bar, you must use one of the prebuilt templates that already conforms to the protocol, such as CPMapTemplate or CPContactTemplate.

Note

The root templates of a tab bar don’t show leading or trailing bar buttons, and the system throws an exception if you attempt to assign bar buttons to the Now Playing template.

## Topics

### Providing Navigation Bar Buttons

var backButton: CPBarButton?

A button to display as the Back button on the navigation bar.

**Required**

var leadingNavigationBarButtons: [CPBarButton]

An array of bar buttons to display on the leading side of the navigation bar.

**Required**

var trailingNavigationBarButtons: [CPBarButton]

An array of bar buttons to display on the trailing side of the navigation bar.

**Required**

class CPBarButton

A button for placement in a navigation bar.

class CPMessageComposeBarButton

A button that activates Siri and initiates the compose message flow.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- CPContactTemplate
- CPGridTemplate
- CPInformationTemplate
- CPListTemplate
- CPMapTemplate
- CPPointOfInterestTemplate

## See Also

### General Purpose Templates

class CPListTemplate

A template that displays and manages a list of items.

class CPGridTemplate

A template that displays and manages a grid of items.

class CPTabBarTemplate

A container template that displays and manages other templates, presenting them as tabs.

class CPTemplate

An abstract base class for interface templates.

