

- os
- OSSignposter
-  withIntervalSignpost(\_:id:\_:around:) 

Instance Method

# withIntervalSignpost(\_:id:\_:around:)

Measures the execution of a closure and attaches the specified message.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func withIntervalSignpost(
    _ name: StaticString,
    id: OSSignpostID = .exclusive,
    _ message: SignpostMetadata,
    around task: () throws -> T
) rethrows -> T
```

## Parameters 

`name`  

The signpost’s name.

`id`  

The signpost’s ID. The default value is exclusive.

`message`  

The interpolated string that the signposter attaches to the signpost. Each of the message’s interpolations can specify individual formatting and privacy options. For more information, see Message Argument Formatters.

`task`  

The closure around which to create the signposted interval.

## Discussion

Important

Don’t create an instance of SignpostMetadata. Instead, provide an interpolated string as the `message` parameter and the system converts it automatically.

The signposter uses a signpost ID to pair the beginning and the end of a signposted interval, which is necessary because multiple intervals with the same configuration and scope can be in-flight simultaneously. If only one interval with a specific configuration can execute at any particular time, pass exclusive as the `id` parameter. Otherwise, use the makeSignpostID() and makeSignpostID(from:) methods to generate a signpost identifier, as the following example shows:

```
let accountNumber = "12345678"

// Create a signposter using the default subsystem.
let signposter = OSSignposter()

// Generate a signpost ID to associate with the signpost.
let signpostID = signposter.makeSignpostID()

// Signpost the interval of a closure that encapsulates
// one or more related tasks, and attach a message that
// securely interpolates sensitive data.
signposter.withIntervalSignpost("Account Reconciliation", id: signpostID,
    "Account: \(accountNumber, privacy: .sensitive(mask: .hash))") {

    // Perform the related tasks.
    processTransactions()
    updateBalance()
}
```

## See Also

### Measuring a Closure

func withIntervalSignpost&lt;T>(StaticString, id: OSSignpostID, around: () throws -> T) rethrows -> T

Measures the execution of the specified closure.

