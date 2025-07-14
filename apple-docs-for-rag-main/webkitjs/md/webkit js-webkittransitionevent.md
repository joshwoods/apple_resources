

- WebKit JS
-  WebKitTransitionEvent 

Class

# WebKitTransitionEvent

`WebKitTransitionEvent` objects provide information about CSS transitions specified using the `transition` property. An event is sent at the end of a transition for each CSS property in the transition. Each event contains the name of the CSS property and duration of the transition. You can use these events to perform some action that starts at the end of a transition.

Safari Desktop 10.0+Safari Mobile 2.0+

``` source
interface WebKitTransitionEvent
```

## Overview

For more on CSS transition events, see https://www.w3.org/TR/css3-transitions/#transition-events.

## Topics

### Accessing Properties

propertyName

The name of the CSS property associated with the transition.

elapsedTime

The duration of the transition, in seconds, since this event was sent. This value is not affected by the value of the CSS `transition-delay` property.

### Initializing

initWebKitTransitionEvent

Initializes a new transition event object.

### Instance Properties

pseudoElement

An abstract element representing the portion of the CSS render tree on which the transition occurs.

## Relationships

### Inherits From

- Event

