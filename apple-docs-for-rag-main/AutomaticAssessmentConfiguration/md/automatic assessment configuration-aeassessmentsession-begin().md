

- Automatic Assessment Configuration
- AEAssessmentSession
-  begin() 

Instance Method

# begin()

Starts an assessment session.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
func begin()
```

## Discussion

After calling the begin() method, wait until the session’s delegate receives the assessmentSessionDidBegin(_:) method before starting an assessment or showing sensitive information. When you’re ready to stop the assessment session, call the end() method.

## See Also

### Starting and stopping a session

func end()

Ends an assessment session.

var isActive: Bool

A Boolean that indicates whether an assessment session is running.

