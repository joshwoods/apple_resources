

- TVML
- Binding and DOM Manipulation
-  needsMoreThreshold 

Article

# needsMoreThreshold

Sets the amount of remaining screen lengths before firing the needs more event.

## Overview

Use the `needsMoreThreshold` attribute to specify when the needs more event is dispatched. When the designated threshold is met, the needs more event requests more data. Here’s an example that dispatches the needs more event when there are fewer than two screen lengths of information in the shelf to display.

```

```

### Values for needsMoreThreshold

Float  
The number of screen lengths of information left before the needs more event is dispatched.

### Elements that Use needsMoreThreshold

- grid

- shelf

- stackTemplate

## See Also

### Binding and DOM Manipulation

binding

Associates information in a data item with an element.

itemID

Mark elements for reuse during DOM updates.

prototype

Associates a data item type with an element.

