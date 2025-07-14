

- RealityKit
- RealityView
-  onCutCommand(perform:) 

Instance Method

# onCutCommand(perform:)

Adds an action to perform in response to the system’s Cut command.

RealityKitSwiftUImacOS 10.15+

``` source
nonisolated
func onCutCommand(perform payloadAction: (() -> [NSItemProvider])?) -> some View
```

## Parameters 

`payloadAction`  

An action closure that should delete the selected data and return NSItemProvider items corresponding to that data, which should be written to the Clipboard. If `action` is `nil`, the Cut command is considered disabled.

## Return Value

A view that triggers `action` when a system Cut command occurs.

