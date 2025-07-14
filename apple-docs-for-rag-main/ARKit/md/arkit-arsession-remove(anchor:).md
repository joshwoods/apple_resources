

- ARKit
- ARSession
-  remove(anchor:) 

Instance Method

# remove(anchor:)

Removes the specified anchor from tracking by the session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func remove(anchor: ARAnchor)
```

## Parameters 

`anchor`  

The anchor to remove.

## Discussion

Changes to anchor tracking take effect when the next frame is captured.

## See Also

### Managing anchors

func add(anchor: ARAnchor)

Adds the specified anchor to be tracked by the session.

