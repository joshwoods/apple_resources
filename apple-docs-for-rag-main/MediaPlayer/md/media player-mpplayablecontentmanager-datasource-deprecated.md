

- Media Player
- MPPlayableContentManager
-  dataSource Deprecated

Instance Property

# dataSource

The data source provided by the app.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
weak var dataSource: (any MPPlayableContentDataSource)? { get set }
```

Deprecated

Use CarPlay framework

## Discussion

This property ensures support for random access of media items through the MPPlayableContentDataSource protocol, whose methods are callable at any point during the app’s lifetime. Set this property as soon as the data is available.

## See Also

### Providing playable content

protocol MPPlayableContentDataSource

The data source providing media metadata to external media players so they can build user interfaces displaying your app’s content.

Deprecated

