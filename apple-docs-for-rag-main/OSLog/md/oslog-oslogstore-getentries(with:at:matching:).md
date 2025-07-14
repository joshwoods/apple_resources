

- OSLog
- OSLogStore
-  getEntries(with:at:matching:) 

Instance Method

# getEntries(with:at:matching:)

Returns a sequence of log entries filtered by the parameters passed in.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func getEntries(
    with options: OSLogEnumerator.Options = [],
    at position: OSLogPosition? = nil,
    matching predicate: NSPredicate? = nil
) throws -> AnySequence
```

