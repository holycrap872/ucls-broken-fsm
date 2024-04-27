# Broken FSM Exercise

This project contains an intentionally broken program. The goal of the exercise
is to fix all of the bugs in the program so it works as expected.

## Repo Details

- `src`: Contains the (broken) source code
- `fsms`: Contains serialized finite state machines
- `.vscode`: Contains setup information for vscode

## Execution Details

To run the program, you need to run the program **with shell** (despite the fact
you're editing it in vscode) and to provide it two things:

1. A serialized finite state machine to execute
2. An input string to see whether the given FSM accepts/rejects it

For example, to run the program on an FSM that determines whether there are an
even number of `1` in a given string, you would :

```
python3 src/fsm/broken_fsm.py --json_fsm fsms/even_ones_fsm.json --input_str "11011"
```
