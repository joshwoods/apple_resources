

- Latent Semantic Mapping
-  LSMResultGetScore(\_:\_:) 

Function

# LSMResultGetScore(\_:\_:)

Returns the likelihood of the specified result.

Mac CatalystmacOS

``` source
func LSMResultGetScore(
    _ result: LSMResult,
    _ n: CFIndex
) -> Float
```

## Discussion

A nan score typically indicates that the category doesn’t contain any token.

## See Also

### Querying Result Information

func LSMResultGetCount(LSMResult) -> CFIndex

Returns the number of results.

func LSMResultGetCategory(LSMResult, CFIndex) -> LSMCategory

Returns the category of the specified result.

