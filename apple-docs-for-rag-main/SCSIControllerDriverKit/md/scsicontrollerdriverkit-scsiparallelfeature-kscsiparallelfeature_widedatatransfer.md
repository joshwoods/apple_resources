

- SCSIControllerDriverKit
- SCSIParallelFeature
-  kSCSIParallelFeature_WideDataTransfer 

Enumeration Case

# kSCSIParallelFeature_WideDataTransfer

The selector for support of wide data transfers.

DriverKit

``` source
kSCSIParallelFeature_WideDataTransfer
```

## Discussion

The framework only supports `Wide16` because the SPI-3 specification obsoleted `Wide32`.

## See Also

### Feature selectors

kSCSIParallelFeature_SynchronousDataTransfer

The selector for support of synchronous data transfers.

kSCSIParallelFeature_QuickArbitrationAndSelection

The selector for support of quick arbitration and selection (QAS).

kSCSIParallelFeature_DoubleTransitionDataTransfers

The selector for support of double transition (DT) data transfers.

kSCSIParallelFeature_InformationUnitTransfers

The selector for SPI information unit (IU) transfers.

kSCSIParallelFeature_TotalFeatureCount

The total number of supported features.

