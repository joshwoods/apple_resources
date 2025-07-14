

- FamilyControls
- FamilyActivitySelection
-  init(from:) 

Initializer

# init(from:)

Creates a new instance by decoding from the given decoder.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

## See Also

### Creating Activity Selections

init()

Creates a new activity selection instance.

