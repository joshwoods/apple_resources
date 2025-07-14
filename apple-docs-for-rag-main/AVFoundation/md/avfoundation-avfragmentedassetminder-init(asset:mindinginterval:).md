

- AVFoundation
- AVFragmentedAssetMinder
-  init(asset:mindingInterval:) 

Initializer

# init(asset:mindingInterval:)

Creates a fragmented asset minder that monitors the specified asset at the indicated minding interval.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    asset: any AVAsset & AVFragmentMinding,
    mindingInterval: TimeInterval
)
```

## Parameters 

`asset`  

The fragmented asset added to the fragmented asset minder.

`mindingInterval`  

The amount of time between checking to see if the system appended additional fragments to the minded asset.

## Return Value

The new fragmented asset minder.

