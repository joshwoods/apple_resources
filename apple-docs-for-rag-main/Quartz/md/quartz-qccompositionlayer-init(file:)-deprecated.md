

- Quartz
- QCCompositionLayer
-  init(file:) Deprecated

Initializer

# init(file:)

Initializes and returns a composition layer using the Quartz Composer composition in the specified file.

macOS 10.5–10.14Deprecated

``` source
init!(file path: String!)
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`path`  

A string that specifies the location of a Quartz Composer composition.

## Return Value

The initialized `QCCompositionLayer` object or `nil` if initialization is not successful.

## See Also

### Creating a Composition Layer

init!(composition: QCComposition!)

Initializes and returns a composition layer using the provided Quartz Composer composition.

Deprecated

