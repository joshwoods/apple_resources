

- Core ML
- MLMetricKey
-  lossValue 

Type Property

# lossValue

The key you use to access the current loss (a `float` value).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class var lossValue: MLMetricKey { get }
```

## Discussion

Use this key to fetch the loss value in the metrics dictionary.

## See Also

### Getting the Keys

class var epochIndex: MLMetricKey

The key you use to access the epoch index (an `Int64` value).

class var miniBatchIndex: MLMetricKey

The key you use to access the mini-batch index (an `Int64` value) within an epoch.

