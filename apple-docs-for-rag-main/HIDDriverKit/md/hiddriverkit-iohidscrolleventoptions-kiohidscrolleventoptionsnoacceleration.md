

- HIDDriverKit
- IOHIDScrollEventOptions
-  kIOHIDScrollEventOptionsNoAcceleration 

Enumeration Case

# kIOHIDScrollEventOptionsNoAcceleration

An option for not applying the default acceleration algorithm to this event.

DriverKitmacOS

``` source
kIOHIDScrollEventOptionsNoAcceleration
```

## Discussion

Scroll events are normally subject to an acceleration algorithm. Use this option if you don’t want to have that acceleration logic applied to the scroll event.

