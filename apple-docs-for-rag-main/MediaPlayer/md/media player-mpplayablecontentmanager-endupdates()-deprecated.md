

- Media Player
- MPPlayableContentManager
-  endUpdates() Deprecated

Instance Method

# endUpdates()

Ends a synchronized update.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func endUpdates()
```

Deprecated

Use CarPlay framework

## Discussion

Call this method upon completion of the batch updates. If you call this method in the middle of an update, all updates stop and you’ll need to apply remaining updates at a later time.

## See Also

### Updating data

func beginUpdates()

Updates several Media Player content items at once.

Deprecated

func reloadData()

Reloads the data from the data source.

Deprecated

