

- Latent Semantic Mapping
-  LSMMapSetStopWords(\_:\_:) 

Function

# LSMMapSetStopWords(\_:\_:)

Specifies which words to omit from all classification efforts.

Mac CatalystmacOS

``` source
func LSMMapSetStopWords(
    _ mapref: LSMMap,
    _ textref: LSMText
) -> OSStatus
```

## Discussion

You must call this function before creating any other texts. The `textref` is no longer needed after this call.

## See Also

### Starting Training Mode

func LSMMapStartTraining(LSMMap) -> OSStatus

Puts the map into training mode, preparing it for the addition of more categories or texts.

func LSMMapAddCategory(LSMMap) -> LSMCategory

Adds another category and returns its category identifier.

func LSMMapGetCategoryCount(LSMMap) -> CFIndex

Returns the number of categories in the map.

func LSMMapAddText(LSMMap, LSMText, LSMCategory) -> OSStatus

Adds a training text to the specified category.

func LSMMapAddTextWithWeight(LSMMap, LSMText, LSMCategory, Float) -> OSStatus

Adds a training text to the specified category with a weight other than 1.

typealias LSMCategory

An integral type that represents a category.

