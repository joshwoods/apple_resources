

- WebKit JS
- WebKitAnimationEvent
-  initWebKitAnimationEvent 

# initWebKitAnimationEvent

Initializes a new animation event object.

``` source
void initWebKitAnimationEvent (in DOMString typeArg, in boolean canBubbleArg, in boolean cancelableArg, in DOMString animationNameArg, in double elapsedTimeArg);
```

## Parameters 

`typeArg`  

The type of event. See Types of Animation Events for possible values.

`canBubbleArg`  

Determines whether the event can bubble. Pass `true` if it can bubble; otherwise, `false`.

`cancelableArg`  

Determines whether the event’s default action can be prevented. Pass `true` if it can be prevented; otherwise, `false`.

`animationNameArg`  

The name of the animation associated with this event.

`elapsedTimeArg`  

The duration of the animation, in seconds, since the event was sent.

## Overview

You use this method to initialize the value of a WebKitTransitionEvent object that is created through the `DocumentEvent` interface. This method can only be invoked before the `WebKitTransitionEvent` object is dispatched via the `dispatchEvent` method (although it can be invoked multiple times during that phase, if necessary). If it is invoked multiple times, the final invocation takes precedence.

