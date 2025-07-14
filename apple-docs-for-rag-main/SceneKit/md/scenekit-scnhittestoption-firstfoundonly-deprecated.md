

- SceneKit
- SCNHitTestOption
-  firstFoundOnly Deprecated

Type Property

# firstFoundOnly

An option to return only the first object found.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let firstFoundOnly: SCNHitTestOption
```

Deprecated

Use the searchMode option with value SCNHitTestSearchMode.any instead.

## Discussion

The value for this key is a NSNumber object containing a Boolean value. The default value is false, specifying that hit-testing should return all objects found. If you specify true, the array of hit-test results contains only the first object found (which is not necessarily the nearest).

## See Also

### Deprecated

static let sortResults: SCNHitTestOption

An option to sort the results of a hit-test.

Deprecated

