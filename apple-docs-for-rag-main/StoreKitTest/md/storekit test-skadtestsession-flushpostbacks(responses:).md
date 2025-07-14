

- StoreKit Test
- SKAdTestSession
-  flushPostbacks(responses:) 

Instance Method

# flushPostbacks(responses:)

Sends the test postbacks and handles the responses.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
func flushPostbacks(responses: @escaping SKANTestPostbackResponseHandler)
```

``` source
func flushPostbacksWithResponses() async throws -> [String : SKAdTestPostbackResponse]
```

## Parameters 

`responses`  

A handler that matches the signature of SKANTestPostbackResponseHandler.

## Discussion

This method sends the test postbacks that you set up using setPostbacks(_:) to the server URL provided in each postback, and then deletes them from this test session. Note that you set up the postback server URL when you create the postback instance using SKAdTestPostback.

This method calls the response handler with either a dictionary that contains postback transactionIdentifier keys with their responses (SKAdTestPostbackResponse), or a single SKAdTestError error. If you receive an error, it indicates a failure that isn’t specific to any single postback, but is a general issue; for example, a test session has no postbacks, there’s a connectivity issue, or the postbacks aren’t registered.

To perform tests with postbacks, do the following:

1.  Create a test postback using SKAdTestPostback.

2.  Add the test postbacks to the test session by calling setPostbacks(_:).

3.  In the code representing the advertised app, register the test postback by calling updatePostbackConversionValue(_:completionHandler:)or registerAppForAdNetworkAttribution().

4.  Optionally, update the conversion value by calling updatePostbackConversionValue(_:completionHandler:).

5.  Call flushPostbacks(responses:) when you’re done updating the conversion value and are ready to test receiving postbacks on your server.

## See Also

### Adding and sending postbacks

func setPostbacks([SKAdTestPostback]) throws

Add test postbacks to the test session.

var postbacks: [SKAdTestPostback]

An array of test postbacks you set in the testing environment.

typealias SKANTestPostbackResponseHandler

A type that represents the test postback response handler.

