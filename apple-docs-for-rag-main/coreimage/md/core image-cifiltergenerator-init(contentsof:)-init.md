

- Core Image
- CIFilterGenerator
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Initializes a filter generator object with the contents of a filter generator file.

macOS 10.5+

``` source
init?(contentsOf aURL: URL)
```

## Parameters 

`aURL`  

The location of a filter generator file.

## Return Value

The initialized `CIFilterGenerator` object. Returns `nil` if the file can’t be read.

## See Also

### Related Documentation

+ filterGeneratorWithContentsOfURL:

Creates and returns a filter generator object and initializes it with the contents of a filter generator file.

+ filterGenerator

Creates and returns an empty filter generator object.

