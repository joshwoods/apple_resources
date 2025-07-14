

- Matter
- MTRBaseClusterServiceArea
-  selectAreas(with:completion:) 

Instance Method

# selectAreas(with:completion:)

Command SelectAreas

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func selectAreas(
    with params: MTRServiceAreaClusterSelectAreasParams,
    completion: @escaping (MTRServiceAreaClusterSelectAreasResponseParams?, (any Error)?) -> Void
)
```

``` source
func selectAreas(with params: MTRServiceAreaClusterSelectAreasParams) async throws -> MTRServiceAreaClusterSelectAreasResponseParams
```

## Discussion

Command used to select a set of device areas, where the device is to operate.

