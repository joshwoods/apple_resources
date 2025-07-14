

- Assignables
- AnonymousUserIdentity
-  init(from:) 

Initializer

# init(from:)

Creates a new instance by decoding from the given decoder.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

## See Also

### Creating an anonymous identity

init()

Initializes an instance of `AnonymousUserIdentity`.

