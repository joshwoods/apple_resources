

- StoreKit Test
- SKAdTestPostback
-  postbackURL 

Instance Property

# postbackURL

A URL on your server where the testing environment sends test postbacks.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var postbackURL: String { get }
```

## Discussion

The testing environment sends the test postback to the postbackURL when you call flushPostbacks(responses:).

Note

Ensure that your test server is running and accepting connections before calling flushPostbacks(responses:).

