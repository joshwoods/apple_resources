

- UIKit
- UIContentView
-  supports(\_:) 

Instance Method

# supports(\_:)

Determines whether the view is compatible with the provided configuration.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 16.0+visionOS

``` source
@MainActor
func supports(_ configuration: any UIContentConfiguration) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`configuration`  

The new configuration to test for compatibility.

## Return Value

true if the view supports this configuration being set to its configuration property and is capable of updating itself for the configuration; otherwise, false.

## Discussion

The default implementation assumes the view is compatible with configuration types that match the type of the view’s existing configuration.

## Default Implementations

### UIContentView Implementations

func supports(any UIContentConfiguration) -> Bool

