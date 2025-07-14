

- Kernel
- Debugging
-  backtrace_user 

Function

# backtrace_user

macOS 10.12+

``` source
unsigned int backtrace_user(uintptr_t *bt, unsigned int btlen, const struct backtrace_control *ctl, struct backtrace_user_info *info_out);
```

## See Also

### Backtrace

backtrace

OSReportWithBacktrace

OSBacktrace

OSPrintBacktrace

