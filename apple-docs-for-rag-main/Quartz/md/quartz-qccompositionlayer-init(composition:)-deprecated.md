

- Quartz
- QCCompositionLayer
-  init(composition:) Deprecated

Initializer

# init(composition:)

Initializes and returns a composition layer using the provided Quartz Composer composition.

macOS 10.5–10.14Deprecated

``` source
init!(composition: QCComposition!)
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`composition`  

The Quartz Composer composition to use as content.

## Return Value

The initialized `QCCompositionLayer` object or `nil` if initialization is not successful.

## See Also

### Creating a Composition Layer

init!(file: String!)

Initializes and returns a composition layer using the Quartz Composer composition in the specified file.

Deprecated

