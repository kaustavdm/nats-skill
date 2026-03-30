# NATS skill for Claude

A Claude Code skill for developing with [NATS](https://nats.io) — the cloud-native messaging system.

The main `SKILL.md` gives Claude the decision-making context for 80% of tasks. The `references/` files are loaded on demand when Claude needs full API details.

## Install

### As a standalone skill

```bash
git clone https://github.com/kaustavdm/nats-skill.git /tmp/nats-skill
cp -r /tmp/nats-skill/skills/nats ~/.claude/skills/nats
```

### As a plugin

TODO

### Verify

Ask Claude: _"What NATS skills do you have?"_

## Coverage

| Area                                                   | Docs                                                                |
| ------------------------------------------------------ | ------------------------------------------------------------------- |
| **Core NATS** — pub/sub, request/reply, queue groups   | <https://docs.nats.io/nats-concepts/core-nats>                      |
| **Subjects** — hierarchies, wildcards (`*`, `>`)       | <https://docs.nats.io/nats-concepts/subjects>                       |
| **JetStream** — streams, consumers, KV, object store   | <https://docs.nats.io/nats-concepts/jetstream>                      |
| **Security** — NKey, JWT/operator, TLS, auth callout   | <https://docs.nats.io/nats-concepts/security>                       |
| **Server** — config, clustering, leaf nodes, embedding | <https://docs.nats.io/running-a-nats-service>                       |
| **Services API** — micro framework, discovery          | <https://docs.nats.io/using-nats/developer/services>                |
| **Subject mapping** — transforms, canary, partitioning | <https://docs.nats.io/nats-concepts/subject_mapping>                |
| **Monitoring** — HTTP endpoints, Prometheus            | <https://docs.nats.io/running-a-nats-service/nats_admin/monitoring> |
| **CLI** — nats pub/sub/stream/consumer/kv commands     | <https://docs.nats.io/using-nats/nats-tools/nats_cli>               |

## Contributing

When adding content, prefer facts sourced from <https://docs.nats.io> and <https://natsbyexample.com>. Include inline source URLs in reference files.

## License

MIT
