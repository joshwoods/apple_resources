

- Local Authentication
- LARightStore
-  shared 

Type Property

# shared

A shared object that stores rights.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class var shared: LARightStore { get }
```

## See Also

### Accessing rights

func right(forIdentifier: String, completion: (LAPersistedRight?, (any Error)?) -> Void)

Fetches a previously stored right from the shared right store.

