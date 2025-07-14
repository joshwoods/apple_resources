

- AVFoundation
- AVCaptureDataOutputSynchronizerDelegate
-  dataOutputSynchronizer(\_:didOutput:) 

Instance Method

# dataOutputSynchronizer(\_:didOutput:)

Provides a collection of synchronized capture data to the delegate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func dataOutputSynchronizer(
    _ synchronizer: AVCaptureDataOutputSynchronizer,
    didOutput synchronizedDataCollection: AVCaptureSynchronizedDataCollection
)
```

**Required**

## Parameters 

`synchronizer`  

The synchronizer object delivering synchronized data.

`synchronizedDataCollection`  

A collection of data samples, one for each capture output governed by the data output synchronizer for which capture data is ready.

## Discussion

Use the data collection’s synchronizedData(for:) method (or equivalent subscript(_:) operator) to retrieve the captured data corresponding to each capture output.

