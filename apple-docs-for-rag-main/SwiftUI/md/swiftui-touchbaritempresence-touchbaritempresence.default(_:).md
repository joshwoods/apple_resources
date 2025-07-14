

- SwiftUI
- TouchBarItemPresence
-  TouchBarItemPresence.default(\_:) 

Case

# TouchBarItemPresence.default(\_:)

The Touch Bar view is visible by default, but can be removed during customization.

macOS 10.15+

``` source
case `default`(String)
```

## Parameters 

`id`  

A globally unique identifier for this item.

## See Also

### Getting presence options

case optional(String)

The Touch Bar view isn’t visible by default, but appears in the customization palette.

case required(String)

The Touch Bar view is visible by default and cannot be removed during customization.

