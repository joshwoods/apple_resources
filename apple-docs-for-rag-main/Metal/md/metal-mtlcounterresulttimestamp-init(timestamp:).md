

- Metal
- MTLCounterResultTimestamp
-  init(timestamp:) 

Initializer

# init(timestamp:)

Creates a timestamp result from a value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(timestamp: UInt64)
```

## Parameters 

`timestamp`  

A timestamp value from a counter sample buffer.

## Discussion

Metal creates MTLCounterResultTimestamp instances for you when you resolve the counter set’s data (see Converting a GPU’s Counter Data into a Readable Format). There’s no reason for you to manually create one in your app.

## See Also

### Swift Support

init()

Creates a default timestamp result.

