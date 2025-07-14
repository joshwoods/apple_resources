

- Metal
- MTLCommandEncoder
-  insertDebugSignpost(\_:) 

Instance Method

# insertDebugSignpost(\_:)

Inserts a debug string into the captured frame data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func insertDebugSignpost(_ string: String)
```

**Required**

## Discussion

For more information, see `Enhancing Frame Capture by Using Labels`.

## See Also

### Annotating the Command Buffer with Debug Information

func pushDebugGroup(String)

Pushes a specific string onto a stack of debug group strings for the command encoder.

**Required**

func popDebugGroup()

Pops the latest string off of a stack of debug group strings for the command encoder.

**Required**

