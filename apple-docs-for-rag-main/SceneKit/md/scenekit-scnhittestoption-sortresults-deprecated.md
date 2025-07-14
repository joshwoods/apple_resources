

- SceneKit
- SCNHitTestOption
-  sortResults Deprecated

Type Property

# sortResults

An option to sort the results of a hit-test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let sortResults: SCNHitTestOption
```

Deprecated

Use the searchMode option with value SCNHitTestSearchMode.all instead.

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value is true, specifying that the array of hit-test results is sorted from nearest to farthest. (When using the hitTestWithSegment(from:to:options:) method, “nearest” is defined as closer to the point specified in the first parameter.) If you specify false, results are returned in an arbitrary order.

## See Also

### Deprecated

static let firstFoundOnly: SCNHitTestOption

An option to return only the first object found.

Deprecated

