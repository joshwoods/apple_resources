

- Swift
- Executor
-  enqueue(\_:) 

Instance Method

# enqueue(\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func enqueue(_ job: consuming ExecutorJob)
```

**Required** Default implementations provided.

## Default Implementations

### Executor Implementations

func enqueue(consuming ExecutorJob)

func enqueue(UnownedJob)

func enqueue(consuming Job)

