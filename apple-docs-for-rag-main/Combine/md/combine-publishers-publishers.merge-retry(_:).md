

- Combine
- Publishers
- Publishers.Merge
-  retry(\_:) 

Instance Method

# retry(\_:)

Attempts to recreate a failed subscription with the upstream publisher up to the number of times you specify.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func retry(_ retries: Int) -> Publishers.Retry
```

## Parameters 

`retries`  

The number of times to attempt to recreate the subscription.

## Return Value

A publisher that attempts to recreate its subscription to a failed upstream publisher.

## Discussion

Use retry(_:) to try a connecting to an upstream publisher after a failed connection attempt.

In the example below, a URLSession.DataTaskPublisher attempts to connect to a remote URL. If the connection attempt succeeds, it publishes the remote service’s HTML to the downstream publisher and completes normally. Otherwise, the retry operator attempts to reestablish the connection. If after three attempts the publisher still can’t connect to the remote URL, the catch(_:) operator replaces the error with a new publisher that publishes a “connection timed out” HTML page. After the downstream subscriber receives the timed out message, the stream completes normally.

```
struct WebSiteData: Codable {
    var rawHTML: String
}

let myURL = URL(string: "https://www.example.com")

cancellable = URLSession.shared.dataTaskPublisher(for: myURL!)
    .retry(3)
    .map({ (page) -> WebSiteData in
        return WebSiteData(rawHTML: String(decoding: page.data, as: UTF8.self))
    })
    .catch { error in
        return Just(WebSiteData(rawHTML: "Unable to load page - timed out."))
}
.sink(receiveCompletion: { print ("completion: \($0)") },
      receiveValue: { print ("value: \($0)") }
 )

// Prints: The HTML content from the remote URL upon a successful connection,
//         or returns "Unable to load page - timed out." if the number of retries exceeds the specified value.
```

After exceeding the specified number of retries, the publisher passes the failure to the downstream receiver.

## See Also

### Handling Errors

func assertNoFailure(String, file: StaticString, line: UInt) -> Publishers.AssertNoFailure&lt;Self>

Raises a fatal error when its upstream publisher fails, and otherwise republishes all received input.

func `catch`&lt;P>((Self.Failure) -> P) -> Publishers.Catch&lt;Self, P>

Handles errors from an upstream publisher by replacing it with another publisher.

func tryCatch&lt;P>((Self.Failure) throws -> P) -> Publishers.TryCatch&lt;Self, P>

Handles errors from an upstream publisher by either replacing it with another publisher or throwing a new error.

