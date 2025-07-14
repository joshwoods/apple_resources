

- Core NFC
- NFCTagCommandConfiguration
-  maximumRetries 

Instance Property

# maximumRetries

The maximum number of retries.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var maximumRetries: Int { get set }
```

## Discussion

You can specify up to 256 retries. By default, the value of this parameter is `0`.

## See Also

### Configuring a Tag Command

var retryInterval: TimeInterval

The time between retries, in seconds.

