

- Latent Semantic Mapping
-  LSMResultGetCategory(\_:\_:) 

Function

# LSMResultGetCategory(\_:\_:)

Returns the category of the specified result.

Mac CatalystmacOS

``` source
func LSMResultGetCategory(
    _ result: LSMResult,
    _ n: CFIndex
) -> LSMCategory
```

## See Also

### Querying Result Information

func LSMResultGetCount(LSMResult) -> CFIndex

Returns the number of results.

func LSMResultGetScore(LSMResult, CFIndex) -> Float

Returns the likelihood of the specified result.

