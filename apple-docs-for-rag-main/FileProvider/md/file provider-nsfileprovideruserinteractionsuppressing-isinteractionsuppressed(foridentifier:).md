

- File Provider
- NSFileProviderUserInteractionSuppressing
-  isInteractionSuppressed(forIdentifier:) 

Instance Method

# isInteractionSuppressed(forIdentifier:)

Asks the File Provider extension if the user suppressed the specified interaction.

macOS 12.0+

``` source
func isInteractionSuppressed(forIdentifier suppressionIdentifier: String) -> Bool
```

**Required**

## Parameters 

`suppressionIdentifier`  

A unique identifier for the user interaction.

## See Also

### Supressing Interactions

func setInteractionSuppressed(Bool, forIdentifier: String)

Tells the File Provider extension that the user wants to suppress the user interaction.

**Required**

