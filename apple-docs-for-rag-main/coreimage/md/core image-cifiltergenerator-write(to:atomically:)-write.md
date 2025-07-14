

- Core Image
- CIFilterGenerator
-  write(to:atomically:) 

Instance Method

# write(to:atomically:)

Archives a filter generator object to a filter generator file.

macOS 10.5+

``` source
func write(
    to aURL: URL,
    atomically flag: Bool
) -> Bool
```

## Parameters 

`aURL`  

A location for the file generator file.

`flag`  

Pass `true` to specify that Core Image should create an interim file to avoid overwriting an existing file.

## Return Value

Returns `true` if the the object is successfully archived to the file.

## Discussion

Use this method to save your filter chain to a file for later use.

