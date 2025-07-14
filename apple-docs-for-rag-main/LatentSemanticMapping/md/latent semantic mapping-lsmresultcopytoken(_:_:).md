

- Latent Semantic Mapping
-  LSMResultCopyToken(\_:\_:) 

Function

# LSMResultCopyToken(\_:\_:)

Returns the token for the n-th best (zero-based) result.

Mac CatalystmacOS

``` source
func LSMResultCopyToken(
    _ result: LSMResult,
    _ n: CFIndex
) -> Unmanaged?
```

## See Also

### Getting a Result

func LSMResultCopyTokenCluster(LSMResult, CFIndex) -> Unmanaged&lt;CFArray>?

Returns the cluster of tokens for the n-th best (zero-based) result.

func LSMResultCopyWord(LSMResult, CFIndex) -> Unmanaged&lt;CFString>?

Returns the word for the n-th best (zero-based) result.

func LSMResultCopyWordCluster(LSMResult, CFIndex) -> Unmanaged&lt;CFArray>?

Returns the cluster of words for the n-th best (zero-based) result.

