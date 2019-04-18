# Semi
##### Lightweight and stupid-simple semantic version bash script.
\
Use Semi to increment major, minor, or patch version numbers as part of a CI/CD workflow.

### Arguments
1) `String` (Optional)
Existing version - Must be formatted as: `0.0.0`

2. `M | m | p` (Optional)
Version part to increment. Defaults to `p`

### Usage Examples

**No arguments**
```bash
sh semi
```

Result: `0.0.1`

**Increment patch version**
When no `version` param exists, patch is used.
```bash
sh semi 8.2.2
```

Result: `8.2.3`

**Increment minor version**
```bash
sh semi 12.2.8 m
```
Result: `12.3.0`

**Increment major version**
```bash
sh semi 12.2.8 M
```
Result: `13.0.0`