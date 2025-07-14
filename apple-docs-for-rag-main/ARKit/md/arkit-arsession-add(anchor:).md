

- ARKit
- ARSession
-  add(anchor:) 

Instance Method

# add(anchor:)

Adds the specified anchor to be tracked by the session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func add(anchor: ARAnchor)
```

## Parameters 

`anchor`  

The anchor to add.

## Discussion

Changes to anchor tracking take effect when the next frame is captured.

## See Also

### Managing anchors

func remove(anchor: ARAnchor)

Removes the specified anchor from tracking by the session.

