

- File Provider
- NSFileProviderUserInteractionSuppressing
-  setInteractionSuppressed(\_:forIdentifier:) 

Instance Method

# setInteractionSuppressed(\_:forIdentifier:)

Tells the File Provider extension that the user wants to suppress the user interaction.

macOS 12.0+

``` source
func setInteractionSuppressed(
    _ suppression: Bool,
    forIdentifier suppressionIdentifier: String
)
```

**Required**

## Parameters 

`suppression`  

A Boolean value that indicates whether the user wants to suppress the specified user interaction.

`suppressionIdentifier`  

A unique identifier for the user interaction.

## See Also

### Supressing Interactions

func isInteractionSuppressed(forIdentifier: String) -> Bool

Asks the File Provider extension if the user suppressed the specified interaction.

**Required**

