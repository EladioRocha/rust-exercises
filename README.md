# Rust Exercises

Two independent Cargo projects for practicing **Rust**: a command-line task manager and a Windows GUI automation experiment.

## Projects

| Directory | What it demonstrates |
| --- | --- |
| [todo-app/](todo-app/) | Console input, structs, task state, and persistence to a text file. |
| [measure-monkey-bot/](measure-monkey-bot/) | Screen/pointer automation using `autogui` and `winapi`. |

Both manifests use the Rust 2018 edition. Install Rust and Cargo before working with either project.

## Task manager

```sh
cd todo-app
cargo check
cargo run
```

The program creates or reads `todo.txt` in the current working directory. At the action prompt, enter:

| Action | Next input |
| --- | --- |
| `create` | Task name. |
| `complete` | Task name to mark complete. |
| `delete` | Task name to remove. |
| `show` | `all`, `completed`, or `todo`. |
| `break` | Exits without requesting another value. |

The interactive prompts remain in Spanish. The storage format uses `task:done` per line; malformed entries or task names containing the separator need additional validation.

## GUI automation experiment

The [measure-monkey-bot manifest](measure-monkey-bot/Cargo.toml) depends on Windows APIs. Review [its entry point](measure-monkey-bot/src/main.rs), coordinates, and platform requirements before running it. Compilation alone does not validate its behavior on your desktop.

## Validation status

These are learning exercises rather than a shared Cargo workspace. Run commands inside the selected project. This documentation update did not execute the GUI automation or establish compatibility with current versions of its dependencies.
