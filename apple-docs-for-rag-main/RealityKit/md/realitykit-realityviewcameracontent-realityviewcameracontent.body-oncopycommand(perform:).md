

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  onCopyCommand(perform:) 

Instance Method

# onCopyCommand(perform:)

Adds an action to perform in response to the system’s Copy command.

RealityKitSwiftUImacOS 10.15+

``` source
nonisolated
func onCopyCommand(perform payloadAction: (() -> [NSItemProvider])?) -> some View
```

## Parameters 

`payloadAction`  

An action closure returning the NSItemProvider items that should be copied to the Clipboard when the Copy command is triggered. If `action` is `nil`, the Copy command is considered disabled.

## Return Value

A view that triggers `action` when a system Copy command occurs.

