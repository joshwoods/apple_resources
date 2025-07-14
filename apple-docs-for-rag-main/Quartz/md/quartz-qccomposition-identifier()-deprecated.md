

- Quartz
- QCComposition
-  identifier() Deprecated

Instance Method

# identifier()

Returns the unique and persistent identifier for the composition from the composition repository.

macOS 10.4–10.15Deprecated

``` source
func identifier() -> String!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The unique identifier for the composition if it comes from the composition repository; `nil` otherwise.

## See Also

### Getting Information About a Composition

func attributes() -> [AnyHashable : Any]!

Returns the attributes of the composition.

Deprecated

func protocols() -> [Any]!

Returns the list of protocols to which the composition conforms.

Deprecated

