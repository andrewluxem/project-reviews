# project-reviews

Builds a decision-ready project review packet from supplied plans, evidence, risks, and actions.

It produces:

- **Project Review Packet:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Project Reviews playbook](https://www.andrewluxem.com/playbooks/project-reviews). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/project-reviews.git
cp -r project-reviews/skills/project-reviews ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r project-reviews/skills/project-reviews ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/project-reviews
/plugin install project-reviews@project-reviews
```

For clients that install from an archive, use the versioned [project-reviews v1.0.0 ZIP](https://www.andrewluxem.com/downloads/project-reviews-v1.0.0.zip).

## Invoke it

```text
Prepare the project review packet from this status evidence
Use the project-reviews skill.
```

Naming the skill is always valid: `use the project-reviews skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/project-reviews/
  assets/project-review-packet-template.md
  LICENSE.md
  meta.yaml
  references/project-review-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/project-reviews/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/project-reviews/LICENSE.md](skills/project-reviews/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.