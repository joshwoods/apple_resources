

- Foundation
- ProgressReporting
-  progress 

Instance Property

# progress

The progress object returned by the class.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var progress: Progress { get }
```

**Required**

## Discussion

The progress object is usually setup at class initialization time and updated as work is completed. The progress property is set only once. If another progress object is needed the caller should create a new instance of the custom class to represent the work.

### Special Considerations

The progress property is only set once.

