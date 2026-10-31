# Second Agent Skills

Credential-free [Agent Skills](https://agentskills.io/specification) for capture, search, PARA triage, onboarding, and handoff with Second.

These skills guide a supported host or the `second` CLI. They do not create credentials, widen OAuth grants, or claim host capabilities the host does not expose. Sign-in stays in your MCP client or CLI config.

## Skills

| Skill | Role |
| --- | --- |
| `second-capture` | Save explicitly supplied URLs or Markdown |
| `second-para` | Search the library and triage with PARA |
| `second-onboarding` | Optional first-use and PARA guidance |
| `second-handoff` | Selected continuation handoff and export/import |

## Requirements

- A supported Second MCP connection (OAuth in the client), **or**
- The `second` CLI with a separately configured account token.

MCP tools and scopes are documented in the [Agent Plugin package](https://2nd.thedevdavid.com/downloads/second-agent-plugin-2.0.0.zip). The skills-only pack does not include `mcp.json` or host setup files.

## Install with skills.sh

```sh
npx skills add thedevdavid/second-skills
```

Or install from the versioned ZIP after it is deployed:

```sh
npx skills add https://2nd.thedevdavid.com/downloads/second-agent-skills-2.0.0.zip
```

- Archive: [https://2nd.thedevdavid.com/downloads/second-agent-skills-2.0.0.zip](https://2nd.thedevdavid.com/downloads/second-agent-skills-2.0.0.zip)
- SHA-256: [https://2nd.thedevdavid.com/downloads/second-agent-skills-2.0.0.zip.sha256.txt](https://2nd.thedevdavid.com/downloads/second-agent-skills-2.0.0.zip.sha256.txt)

## Agent Plugin (MCP + skills)

Hosts that want the remote MCP address bundled with the same skills should use the [Agent Plugin ZIP](https://2nd.thedevdavid.com/downloads/second-agent-plugin-2.0.0.zip) instead.

## License

MIT. See [LICENSE](./LICENSE).
