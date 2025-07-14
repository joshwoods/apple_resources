

- Foundation
- NSEnumerationOptions
-  concurrent 

Type Property

# concurrent

Specifies that the Block enumeration should be concurrent.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var concurrent: NSEnumerationOptions { get }
```

## Discussion

The order of invocation is nondeterministic and undefined; this flag is a hint and may be ignored by the implementation under some circumstances; the code of the Block must be safe against concurrent invocation.

## See Also

### Constants

static var reverse: NSEnumerationOptions

Specifies that the enumeration should be performed in reverse.

