

- StoreKit Test
- SKAdTestSession
-  postbacks 

Instance Property

# postbacks

An array of test postbacks you set in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
var postbacks: [SKAdTestPostback] { get }
```

## Discussion

Use this property to check that your updates to the test postbacks, such as conversion value updates, are working as expected. See setPostbacks(_:) for information on adding postbacks to the test session.

## See Also

### Adding and sending postbacks

func setPostbacks([SKAdTestPostback]) throws

Add test postbacks to the test session.

func flushPostbacks(responses: SKANTestPostbackResponseHandler)

Sends the test postbacks and handles the responses.

typealias SKANTestPostbackResponseHandler

A type that represents the test postback response handler.

