

- SwiftUI
- TouchBarItemPresence
-  TouchBarItemPresence.required(\_:) 

Case

# TouchBarItemPresence.required(\_:)

The Touch Bar view is visible by default and cannot be removed during customization.

macOS 10.15+

``` source
case required(String)
```

## Parameters 

`id`  

A globally unique identifier for this item.

## See Also

### Getting presence options

case `default`(String)

The Touch Bar view is visible by default, but can be removed during customization.

case optional(String)

The Touch Bar view isn’t visible by default, but appears in the customization palette.

