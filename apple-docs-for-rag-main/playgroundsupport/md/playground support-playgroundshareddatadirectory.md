

- Playground Support
-  playgroundSharedDataDirectory 

Global Variable

# playgroundSharedDataDirectory

The path to the directory containing data shared between all playgrounds in Xcode.

macOS 11.0+Xcode 12.0+

``` source
let playgroundSharedDataDirectory: URL
```

## Discussion

Use this directory to store data that must be persisted between playground runs or shared between multiple playgrounds.

## See Also

### Data Persistence

class PlaygroundKeyValueStore

A data storage container you use to persist information across different sessions.

enum PlaygroundValue

The types you can save in the key-value store or send in messages to live views.

