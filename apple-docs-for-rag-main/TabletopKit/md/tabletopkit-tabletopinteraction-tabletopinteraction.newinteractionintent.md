

- TabletopKit
- TabletopInteraction
-  TabletopInteraction.NewInteractionIntent 

Enumeration

# TabletopInteraction.NewInteractionIntent

The possible outcomes when a new interaction is about to be started.

visionOS 2.2+

``` source
enum NewInteractionIntent
```

## Topics

### Enumeration Cases

case acceptWithConfiguration(TabletopInteraction.Configuration)

Accept the new interaction and provide the initial configuration.

case reject

Reject the new interaction.

