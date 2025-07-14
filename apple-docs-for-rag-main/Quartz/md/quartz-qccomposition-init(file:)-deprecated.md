

- Quartz
- QCComposition
-  init(file:) Deprecated

Initializer

# init(file:)

Returns a composition object initialized with a Quartz Composer composition file.

macOS 10.4–10.15Deprecated

``` source
init!(file path: String!)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`path`  

A path to a file created with the Quartz Composer developer tool (`.qtz` extension).

## Return Value

A Quartz Composer composition object or `nil` if there is an error.

## See Also

### Creating a Composition

init!(data: Data!)

Returns a composition object initialized with the contents of a Quartz Composer composition file.

Deprecated

