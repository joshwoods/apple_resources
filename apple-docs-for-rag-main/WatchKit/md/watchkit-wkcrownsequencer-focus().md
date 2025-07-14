

- WatchKit
- WKCrownSequencer
-  focus() 

Instance Method

# focus()

Begins the delivery of crown events to the current crown sequencer.

watchOS 3.0+

``` source
func focus()
```

## Discussion

You must call this method to begin the delivery of crown events to your crown sequencer object. If your interface includes a picker or scrollable scene that is currently receiving crown events, calling this method causes that object to resign focus.

## See Also

### Managing the Focus

func resignFocus()

Ends the delivery of crown events to the current crown sequencer.

