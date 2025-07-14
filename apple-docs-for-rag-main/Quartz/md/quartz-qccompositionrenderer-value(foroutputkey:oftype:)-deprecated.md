

- Quartz
- QCCompositionRenderer
-  value(forOutputKey:ofType:) Deprecated

Instance Method

# value(forOutputKey:ofType:)

Returns the current value on an output port (identified by its key) of the root patch of the composition.

macOS 10.4–10.15Deprecated

``` source
func value(
    forOutputKey key: String!,
    ofType type: String!
) -> Any!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`key`  

The key associated with an output port for the root patch of a composition. This method throws an exception if `key` is invalid.

`type`  

A string that specifies the class.

## Return Value

The value.

## Discussion

The value type depends on the type of the port type, as shown in the following table

| Port type | Value type |
|----|----|
| Boolean, Index, or Number | NSNumber or any object that responds to the methods `integerValue`, `floatValue`, or `doubleValue` |
| String | NSString or any object that responds to the methods`stringValue` or `description` |
| Color | NSColor, CIColor, or `CGColor` object |
| Image | NSImage, NSBitmapImageRep, `CGImage` object, CIImage, `CVPixelBuffer` object, `CVOpenGLBuffer` object, or an opaque `QCImage` (that is, an optimized abstract image object only to be used with `setValue:forInputKey:` of another ``) |
| Structure | NSArray or NSDictionary |

## See Also

### Passing and Retrieving Values From a Composition

func setValue(Any!, forInputKey: String!) -> Bool

Sets the value for an input port of a composition.

**Required**

Deprecated

func value(forInputKey: String!) -> Any!

Returns the value for an input port of a composition.

**Required**

Deprecated

func value(forOutputKey: String!) -> Any!

Returns the value for an output port of a composition.

**Required**

Deprecated

