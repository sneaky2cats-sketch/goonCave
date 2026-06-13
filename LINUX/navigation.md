# Navigation Commands

## Directory Shortcuts

```bash
.       # current directory
..      # parent directory (one level up)
/       # root directory (works from anywhere)
```

## Changing Directories

```bash
cd /                # go to root directory (absolute path, works from anywhere)
cd ..               # go up ONE level (to parent directory)
cd ../..            # go up TWO levels (no spaces between dots)
# Each .. = one level up
```

**Example:**
- If you're at: `/home/user/documents/projects/`
- `cd ..` takes you to: `/home/user/documents/`
- `cd ../..` takes you to: `/home/user/`
- `cd /` takes you to: `/` (root, from anywhere)

## Listing Files and Directories

```bash
ls -l                   # list everything with permissions
ls -l fileName          # show specific file with permissions
ls -l Documents         # show contents inside Documents with permissions
ls -d Documents         # show Documents folder itself (not contents)
                        # useful when you want info about the folder, not its contents
```

**Key difference with `-d` flag:**
- **With `-d`**: shows the folder's own permissions/properties
- **Without `-d`**: shows what's INSIDE the folder

---

**Book Reference:** Linux Basics for Hackers - Chapter 1
