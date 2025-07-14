

- StoreKit Test
-  SKANTestPostbackResponseHandler 

Type Alias

# SKANTestPostbackResponseHandler

A type that represents the test postback response handler.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
typealias SKANTestPostbackResponseHandler = ([String : SKAdTestPostbackResponse]?, (any Error)?) -> Void
```

## Discussion

The system calls the response handler and provides one of two values:

- A dictionary with a key that identifies a test postback using its transactionIdentifier value, and the associated value of the response, SKAdTestPostbackResponse that you receive when calling flushPostbacks(responses:)

- An SKAdTestError error

## See Also

### Adding and sending postbacks

func setPostbacks([SKAdTestPostback]) throws

Add test postbacks to the test session.

var postbacks: [SKAdTestPostback]

An array of test postbacks you set in the testing environment.

func flushPostbacks(responses: SKANTestPostbackResponseHandler)

Sends the test postbacks and handles the responses.

