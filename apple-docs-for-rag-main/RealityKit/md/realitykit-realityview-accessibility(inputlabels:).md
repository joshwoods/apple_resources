

- RealityKit
- RealityView
-  accessibility(inputLabels:) 

Instance Method

# accessibility(inputLabels:)

Sets alternate input labels with which users identify a view.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac CatalystmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 6.0+

``` source
nonisolated
func accessibility(inputLabels: [Text]) -> ModifiedContent
```

## Parameters 

`inputLabels`  

An array of Text elements to use as input labels.

## Discussion

Provide labels in descending order of importance. Voice Control and Full Keyboard Access use the input labels.

Note

If you don’t specify any input labels, the user can still refer to the view using the accessibility label that you add with the accessibility(label:) modifier.

