

- Video Subscriber Account
- VSAccountManagerResult
-  cancel() 

Instance Method

# cancel()

Cancels an in-progress request for subscriber account information.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
func cancel()
```

## Discussion

Your app uses this method to notify a VSAccountManager instance to cancel the current request for subscriber account information. No guarantees are made that the cancellation request will succeed or finish immediately.

