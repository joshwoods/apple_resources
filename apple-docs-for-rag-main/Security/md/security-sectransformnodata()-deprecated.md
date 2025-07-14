

- Security
-  SecTransformNoData() Deprecated

Function

# SecTransformNoData()

Returns an object from inside a ProcessData override that says that although no data is being returned the transform is still active and awaiting data.

macOS 10.7–13.0Deprecated

``` source
func SecTransformNoData() -> CFTypeRef
```

Deprecated

SecTransform is no longer supported

## Return Value

A ‘special’ value that allows that specifies that the transform is still active and awaiting data.

## Discussion

The standard behavior for the ProcessData override is that it will receive a CFData object and it processes that data and returns another data object that contains the processed data. When there is no more data to process the ProcessData override block is called one last time with a `NULL` data reference. The ProcessData block should/must return the `NULL` data reference to complete the processing. This model does not work well for some transforms. For example a digest transform needs to see ALL of the data that is being digested before it can send out the digest value.

If a ProcessData block has no data to return, it can return SecTransformNoData(), which informs the transform system that there is no data to pass on to the next transform.

