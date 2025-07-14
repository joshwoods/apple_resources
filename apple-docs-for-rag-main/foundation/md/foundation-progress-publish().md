

- Foundation
- Progress
-  publish() 

Instance Method

# publish()

Publishes the progress object for other processes to observe it.

macOS 10.9+

``` source
func publish()
```

## Discussion

Entries in the user info dictionary determine whether another process can discover the progress object to observe it, and how it does that. For example, a fileURLKey entry makes a progress object discoverable by corresponding invokers of addSubscriber(forFileURL:withPublishingHandler:). The system constrains access to the published progress URL with your app sandbox. If you can’t see the file due to the app’s sandbox restrictions, you can’t observe the progress on it.

When you make a progress object observable by other processes, you must ensure that at least localizedDescription, isIndeterminate, and fractionCompleted always work when you send proxies of your progress object in other processes. You make isIndeterminate and fractionCompleted work by accurately setting the total and completed unit counts of the progress. You make localizedDescription work by setting the value of the kind property to something valid, like file, and then fulfilling the requirements for that kind of progress.

You can instead set the value of localizedDescription directly, but that’s not perfectly reliable because other processes might be using a different localization than yours.

You can publish an instance of Progress one time only.

## See Also

### Reporting Progress to Other Processes

func unpublish()

Removes a progress object from publication, making it unobservable by other processes.

