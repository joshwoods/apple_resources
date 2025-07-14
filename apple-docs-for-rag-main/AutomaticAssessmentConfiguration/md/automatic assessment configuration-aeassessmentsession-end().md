

- Automatic Assessment Configuration
- AEAssessmentSession
-  end() 

Instance Method

# end()

Ends an assessment session.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
func end()
```

## Discussion

Before calling the end() method, be sure to stop the assessment and hide any sensitive information. After calling the method, wait until the session’s delegate receives the assessmentSessionDidEnd(_:) method before you report the assessment as complete to the user.

## See Also

### Starting and stopping a session

func begin()

Starts an assessment session.

var isActive: Bool

A Boolean that indicates whether an assessment session is running.

