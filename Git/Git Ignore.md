Create a `.gitignore` file in the root directory of your project

```gitignore
# Ignore all .log files
*.log

# Ignore the 'node_modules' directory
node_modules/

# Ignore all files named 'temp.txt'
temp.txt
```

### Common patterns to ignore
- **Build artifacts:** `bin/`, `out/`, `dist/`
- **Log files:** `*.log`, `*.log.*`
- **Temporary files:** `*.tmp`, `*.bak`, `*~`
- **IDE-specific files:** `.idea/`, `.vscode/`
- **OS-specific files:** `.DS_Store` (macOS)