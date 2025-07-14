

- Objective-C Runtime
- NXHashTablePrototype
-  init(hash:isEqual:free:style:) 

Initializer

# init(hash:isEqual:free:style:)

Mac CatalystmacOS

``` source
init(
    hash: (UnsafeRawPointer?, UnsafeRawPointer?) -> UInt,
    isEqual: (UnsafeRawPointer?, UnsafeRawPointer?, UnsafeRawPointer?) -> Int32,
    free: (UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void,
    style: Int32
)
```

