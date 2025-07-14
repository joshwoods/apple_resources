

- TVML
- Binding and DOM Manipulation
-  itemID 

Article

# itemID

Mark elements for reuse during DOM updates.

## Overview

Use the `itemID` attribute to identify which elements are considered the same so they can be reused during DOM updates. When recreating the DOM, TVMLKit makes any necessary changes at the view level while retaining existing cells that have not been modified.

### Values for itemID

String  
The identifier for the item. The identifier must be unique inside its parent DOM element. The identifier does not have to be unique inside of the document.

### Elements that Use itemID

- productBundleTemplate

- productTemplate

- searchTemplate

- stackTemplate

`itemID` can only be used with the following elements inside of the above templates:

- grid

- section in the `grid` or `shelf` element

- shelf

- Any element that can appear in a `shelf`/`section` or `grid`/`section` combination

## See Also

### Binding and DOM Manipulation

binding

Associates information in a data item with an element.

prototype

Associates a data item type with an element.

needsMoreThreshold

Sets the amount of remaining screen lengths before firing the needs more event.

