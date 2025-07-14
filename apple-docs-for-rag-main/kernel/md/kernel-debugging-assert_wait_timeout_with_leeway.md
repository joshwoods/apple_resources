

- Kernel
- Debugging
-  assert_wait_timeout_with_leeway 

Function

# assert_wait_timeout_with_leeway

macOS 10.9+

``` source
wait_result_t assert_wait_timeout_with_leeway(event_t event, wait_interrupt_t interruptible, wait_timeout_urgency_t urgency, uint32_t interval, uint32_t leeway, uint32_t scale_factor);
```

## See Also

### Assertions

Assert

assert_wait

assert_wait_deadline

assert_wait_deadline_with_leeway

assert_wait_timeout

