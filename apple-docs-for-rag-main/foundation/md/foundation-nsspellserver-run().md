

- Foundation
- NSSpellServer
-  run() 

Instance Method

# run()

Causes the receiver to start listening for spell-checking requests.

Mac Catalyst 13.0+macOS 10.0+

``` source
func run()
```

## Discussion

This method starts a loop that never returns; you need to set the `NSSpellServer` object’s delegate before sending this message.

## See Also

### Related Documentation

var delegate: (any NSSpellServerDelegate)?

Returns the receiver’s delegate.

### Providing Spelling Services

func registerLanguage(String?, byVendor: String?) -> Bool

Notifies the receiver of a language your spelling checker can check.

