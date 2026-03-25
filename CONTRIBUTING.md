# Contributing

Thanks for your interest in contributing to Visual Research.

## How the skill works

`SKILL.md` is the entire skill — Claude Code reads it when the skill is invoked. The `references/` folder contains supporting docs that the skill reads during execution. The `templates/` folder has the HTML report template.

There's no build step, no runtime, no tests. The "code" is the prompt.

## What to change where

| Change | File |
|--------|------|
| Pipeline logic, phases, tool usage | `SKILL.md` |
| Report layout, styling, sections | `templates/report.html` |
| Research methodology | `references/brand-audit-framework.md` |
| Search strategies for finding assets | `references/source-discovery-guide.md` |
| Image extraction (Instagram, YouTube, etc.) | `references/image-extraction-techniques.md` |
| Report design rules | `references/ce-styleguide.md` |

## Testing changes

1. Copy the skill to your Claude Code skills directory:
   ```bash
   cp -r . ~/.claude/skills/visual-research
   ```
2. Open Claude Code and run: `research [any brand]`
3. Check the generated HTML report opens correctly in a browser

## Submitting a PR

- Keep changes focused — one concern per PR
- If you're changing `SKILL.md`, describe which phase is affected
- If you're changing the template, include a screenshot of a generated report

## Reporting issues

Open an issue on GitHub. Include:
- What brand you were researching
- Which phase failed (Discover, Capture, Extract, Analyze, or Package)
- The error or unexpected behavior
