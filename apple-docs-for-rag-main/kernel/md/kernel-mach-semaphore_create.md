

- Kernel
- mach
-  semaphore_create 

Function

# semaphore_create

macOS 10.0+

``` source
kern_return_t semaphore_create(task_t task, semaphore_t *semaphore, int policy, int value);
```

## See Also

### Semaphore

semaphore_destroy

semaphore_signal

semaphore_signal_all

semaphore_wait

semaphore_wait_deadline

semaphore_wait_noblock

