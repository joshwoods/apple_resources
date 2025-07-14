

- WatchKit
- WKCrownSequencer
-  resignFocus() 

Instance Method

# resignFocus()

Ends the delivery of crown events to the current crown sequencer.

watchOS 3.0+

``` source
func resignFocus()
```

## Discussion

Call this method when you no longer want to receive crown events in the current crown sequencer. If the user taps a picker object or a scrollable scene in your interface, the system automatically removes the focus from any active crown sequencer.

## See Also

### Managing the Focus

func focus()

Begins the delivery of crown events to the current crown sequencer.

