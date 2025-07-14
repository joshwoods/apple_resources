

- Swift
- Executor
-  enqueue(\_:) Deprecated

Instance Method

# enqueue(\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func enqueue(_ job: consuming Job)
```

**Required** Default implementations provided.

Deprecated

Implement 'enqueue(\_: consuming ExecutorJob)' instead

## Default Implementations

### Executor Implementations

func enqueue(consuming Job)

func enqueue(UnownedJob)

func enqueue(consuming ExecutorJob)

