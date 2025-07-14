

- AppKit
- NSUserInterfaceCompression
-  compress(withPrioritizedCompressionOptions:) 

Instance Method

# compress(withPrioritizedCompressionOptions:)

Compress the view by applying the specified compression options.

macOS 10.13+

``` source
func compress(withPrioritizedCompressionOptions prioritizedOptions: [NSUserInterfaceCompressionOptions])
```

**Required**

## Parameters 

`prioritizedOptions`  

An array of compression options that the view should apply to reduce its size.

## Discussion

When the system calls this method, the view should resize itself according to the compression options supplied.

Compression options that are handled by the system are not included in the supplied array.

