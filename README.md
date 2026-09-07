# filewarden

Small Go tool: declutter ~/Downloads in one command

Started as a weekend hack, grew on me.

## Examples

```bash
./bin/filewarden ~/Downloads --dry-run
./bin/filewarden ~/Downloads
```

## Install

```bash
go build -o bin/ ./...
```

## Features

- Single static binary, no runtime deps
- Dry-run prints the plan before moving anything
- Groups files into folders by extension
- Skips hidden files and folders by default

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   └── usage.md
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── go.mod
└── main.go
```

## Development

```bash
go build ./...
go vet ./...
```

## Notes

- mostly stable, edge cases remain
