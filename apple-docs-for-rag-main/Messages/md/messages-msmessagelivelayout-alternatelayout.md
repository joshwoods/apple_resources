

- Messages
- MSMessageLiveLayout
-  alternateLayout 

Instance Property

# alternateLayout

A template layout to be displayed when the live layout is unavailable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var alternateLayout: MSMessageTemplateLayout { get }
```

## Discussion

To display the live layout, the device must be running iOS 11 or later, and must have your iMessage app installed. All other devices, including devices that do not support iMessage apps (macOS, iOS 9 and earlier, and SMS devices), use the alternate layout.

