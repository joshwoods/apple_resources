

- SCSIControllerDriverKit
- SCSIParallelFeature
-  kSCSIParallelFeature_TotalFeatureCount 

Enumeration Case

# kSCSIParallelFeature_TotalFeatureCount

The total number of supported features.

DriverKit

``` source
kSCSIParallelFeature_TotalFeatureCount
```

## Discussion

This is the last member of the SCSIParallelFeature enumeration. Since the enumeration is zero-based, this value always represents the correct total number of features.

## See Also

### Feature selectors

kSCSIParallelFeature_WideDataTransfer

The selector for support of wide data transfers.

kSCSIParallelFeature_SynchronousDataTransfer

The selector for support of synchronous data transfers.

kSCSIParallelFeature_QuickArbitrationAndSelection

The selector for support of quick arbitration and selection (QAS).

kSCSIParallelFeature_DoubleTransitionDataTransfers

The selector for support of double transition (DT) data transfers.

kSCSIParallelFeature_InformationUnitTransfers

The selector for SPI information unit (IU) transfers.

