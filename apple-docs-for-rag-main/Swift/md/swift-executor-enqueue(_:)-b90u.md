

- Swift
- Executor
-  enqueue(\_:) 

Instance Method

# enqueue(\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func enqueue(_ job: UnownedJob)
```

**Required** Default implementations provided.

## Default Implementations

### Executor Implementations

func enqueue(consuming ExecutorJob)

func enqueue(consuming Job)

func enqueue(UnownedJob)

