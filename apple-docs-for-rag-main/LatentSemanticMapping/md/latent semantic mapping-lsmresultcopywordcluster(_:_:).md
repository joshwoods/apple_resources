

- Latent Semantic Mapping
-  LSMResultCopyWordCluster(\_:\_:) 

Function

# LSMResultCopyWordCluster(\_:\_:)

Returns the cluster of words for the n-th best (zero-based) result.

Mac CatalystmacOS

``` source
func LSMResultCopyWordCluster(
    _ result: LSMResult,
    _ n: CFIndex
) -> Unmanaged?
```

## See Also

### Getting a Result

func LSMResultCopyToken(LSMResult, CFIndex) -> Unmanaged&lt;CFData>?

Returns the token for the n-th best (zero-based) result.

func LSMResultCopyTokenCluster(LSMResult, CFIndex) -> Unmanaged&lt;CFArray>?

Returns the cluster of tokens for the n-th best (zero-based) result.

func LSMResultCopyWord(LSMResult, CFIndex) -> Unmanaged&lt;CFString>?

Returns the word for the n-th best (zero-based) result.

