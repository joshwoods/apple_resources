

- HealthKit
- HKAppleWalkingSteadinessClassification
-  maximum 

Instance Property

# maximum

The minimum walking steadiness percentage for the classification.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOSwatchOS 8.0+

``` source
var maximum: HKQuantity { get }
```

## Discussion

This property contains the minimum walking steadiness value for the classification. It contains an HKQuantity instance with a percentage value between `0.0` and `1.0`.

