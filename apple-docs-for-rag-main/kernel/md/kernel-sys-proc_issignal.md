

- Kernel
- sys
-  proc_issignal 

Function

# proc_issignal

macOS 10.4+

``` source
int proc_issignal(int pid, sigset_t mask);
```

## See Also

### proc

proc_best_name

proc_chrooted

proc_csflags

proc_exiting

proc_find

proc_forcequota

proc_gettty

proc_gettty_dev

proc_in_teardown

proc_is64bit

proc_is64bit_data

proc_is_classic

proc_isinferior

proc_issetugid

proc_name

proc_noremotehang

proc_original_ppid

proc_pgrpid

Get the process group id for the passed-in process.

proc_pid

proc_platform

proc_ppid

proc_rele

proc_sdk

proc_self

proc_selfcsflags

proc_selfname

proc_selfpgrpid

Get the process group id for the current process, as with proc_pgrpid().

proc_selfpid

proc_selfppid

proc_send_synchronous_EXC_RESOURCE

proc_sessionid

proc_signal

proc_suser

proc_tbe

proc_ucredDeprecated

current_proc

current_proc_EXTERNAL

