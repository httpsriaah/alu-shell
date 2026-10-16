# processes_and_signals

Bash scripts on Linux processes, PIDs and signals.

## Learning objectives

- **PID**: a unique number the kernel assigns to every running process.
- **Process**: a running instance of a program, with its own PID, memory and state.
- **Finding a PID**: `ps`, `pgrep <name>`, or `echo $$` for the current shell.
- **Killing a process**: `kill <PID>`, `pkill <name>`, or `killall <name>`.
- **Signal**: an asynchronous notification sent to a process (e.g. SIGINT, SIGTERM). A process can handle most with `trap`.
- **Signals that cannot be ignored**: SIGKILL (9) and SIGSTOP.

## Files

| File | Description |
|------|-------------|
| 0-what-is-my-pid | Displays its own PID |
| 1-list_your_processes | Lists all processes in user format with hierarchy |
| 2-show_your_bash_pid | Shows lines containing bash (via ps) |
| 3-show_your_bash_pid_made_easy | Shows PID and name of bash processes (no ps) |
| 4-to_infinity_and_beyond | Prints a message forever |
| 5-dont_stop_me_now | Stops script 4 with kill |
| 6-stop_me_if_you_can | Stops script 4 without kill/killall |
| 7-highlander | Resists SIGTERM |
| 67-stop_me_if_you_can | Sends SIGTERM to 7-highlander |
| 8-beheaded_process | Kills 7-highlander with SIGKILL |
| 10-process_and_pid_file | PID file plus SIGINT/SIGTERM/SIGQUIT handling |
| manage_my_process | Writes "I am alive!" to /tmp/my_process forever |
| 11-manage_my_process | Init script: start, stop, restart |
