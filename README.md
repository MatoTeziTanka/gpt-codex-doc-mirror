# GPT Codex Doc Mirror

Mirror [GPT Codex documentation](https://developers.openai.com/codex/) locally with automatic change detection and changelog generation.

**GitHub:** https://github.com/MatoTeziTanka/gpt-codex-doc-mirror

## Setup

```bash
git clone https://github.com/MatoTeziTanka/gpt-codex-doc-mirror.git
cd gpt-codex-doc-mirror
chmod +x bin/codex-docs-sync.sh
mkdir -p data/gpt-codex logs
./bin/codex-docs-sync.sh
```

## Configuration

| Variable | Default | Description |
|----------|---------|-------------|
| `DOC_MIRROR_BASE` | `.` | Root directory |
| `GRAPH` | (empty) | Optional JSONL knowledge graph |

## Usage

```bash
./bin/codex-docs-sync.sh          # Normal sync
./bin/codex-docs-sync.sh --force  # Force re-download
```

## License

MIT
