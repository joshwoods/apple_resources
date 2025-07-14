

- AVFoundation
- AVCaptureIndexPicker
-  selectedIndex 

Instance Property

# selectedIndex

The currently selected index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var selectedIndex: Int { get set }
```

## Discussion

The default value is `0`. You can only set a value that’s greater than or equal to `0` and less than numberOfIndexes.

Important

Only modify the selected index from the same dispatch queue that you specified in the control’s setActionQueue:action: method.

## See Also

### Accessing the control value

var numberOfIndexes: Int

The number of index values the control provides.

