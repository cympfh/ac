# ac

AtCoder CommandLine Alias (w/ cargo-atcoder)

## Installation

Copy `bin/ac` or Clone this repository and PATH to it.
Please `chmod +x` if need.

```bash
# For Example:
git clone git@github.com:cympfh/ac.git ~/git/ac
export PATH=$PATH:~/git/ac/bin
```

## Requirement

This uses [cargo-atcoder](https://github.com/tanakh/cargo-atcoder).

## Usage

```bash
ac new <CONTEST_ID> [OPTIONS]
    Alias for `cargo atcoder new <CONTEST_ID> [OPTIONS]`

# Under the Contest Directory
ac test <PROBLEM_ID>
    Alias for `cargo atcoder test <PROBLEM_ID>`

ac test
    `PROBLEM_ID` will be the one just you have tested (with `ac test ...`).

ac test <PROBLEM_ID> <CASE_ID>
    Alias for `cargo atcoder test <PROBLEM_ID> <CASE_ID>`

ac test <PROBLEM_ID> -
    Test with `stdin`

ac test <PROBLEM_ID> <INPUT_FILE_PATH>
    Test with `<INPUT_FILE_PATH>`.
    where `INPUT_FILE_PATH` should NOT be `-`, `1`, `2` or ...

ac submit <PROBLEM_ID> [OPTIONS]
    Alias for `cargo atcoder submit <PROBLEM_ID> [OPTIONS]`

ac submit
    `PROBLEM_ID` will be the one just you have tested (with `ac test`).

ac status
    Alias for `cargo atcoder status`

ac edit <PROBLEM_ID>
    Open `src/bin/<PROBLEM_ID>.rs` with \$EDITOR
```
