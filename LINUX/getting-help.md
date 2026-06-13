# Getting Help in Linux

## Main Help Commands

```bash
command --help              # most reliable flag (works on almost everything)
man command                 # detailed manual pages
help command                # bash built-in help (bash only, not zsh)
```

## Shell-Specific Help

### Running bash help in zsh (without switching shells)

```bash
bash -c "help command"      # run bash help while staying in zsh
# Example: bash -c "help cd"
```

**What this does:**
- Opens a bash subshell temporarily
- Runs the help command
- Shows output
- Returns to your current shell (zsh)

### Other help variations

```bash
command -h              # sometimes works, but not always
                        # some commands use -h for something else (like "human readable")
                        # stick with --help instead
```

## Tips

- **Most reliable:** Use `--help` or `man command`
- **`help` command:** Only works for shell built-ins (cd, echo, alias, etc)
- **`man` pages:** Great for in-depth information, press `q` to exit

---

**Book Reference:** Linux Basics for Hackers - Chapter 1
