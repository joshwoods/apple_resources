

- HIDDriverKit
- IOHIDKeyboardEventOptions
-  kIOHIDKeyboardEventOptionsNoKeyRepeat 

Enumeration Case

# kIOHIDKeyboardEventOptionsNoKeyRepeat

An option for not applying the default key repeat logic to the event.

DriverKitmacOS

``` source
kIOHIDKeyboardEventOptionsNoKeyRepeat
```

## Discussion

The default behavior for keyboard events is to repeat keys if the user holds down the key for the amount of time defined in system preferences. Use this option to disable this behavior for the event.

