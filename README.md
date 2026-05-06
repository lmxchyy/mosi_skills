# mosi_skills

Codex skills collection for marketing and content workflows.

This repository currently includes a reusable marketing copywriting skill that helps create, critique, and optimize high-converting copy for ads, landing pages, social posts, short video scripts, emails, and product launches.

## Skills

### marketing-copywriting

Path: `marketing-copywriting/`

Use this skill when you need conversion-oriented copywriting, such as:

- Xiaohongshu marketing copy
- Product launch copy
- Landing page sections
- Social ad copy
- Short video scripts
- Email promotions
- Pain-point hooks and CTA optimization
- Chinese or English direct-response copy

The skill follows a practical conversion structure:

1. Identify the buyer, product, offer, channel, and desired action.
2. Extract the user's pain point, desired identity shift, objection, proof, and urgency.
3. Draft with `Hook -> Bridge -> CTA`.
4. Tighten the copy with concrete scenes, outcome language, and one clear next step.
5. Provide variants when useful.

## Repository Structure

```text
mosi_skills/
  marketing-copywriting/
    SKILL.md
    agents/
      openai.yaml
    marketing copywriting template image
```

## Install

Install the skill into Codex from GitHub:

```bash
python install-skill-from-github.py --repo lmxchyy/mosi_skills --path marketing-copywriting
```

Or copy the `marketing-copywriting` directory into your local Codex skills directory:

```text
~/.codex/skills/marketing-copywriting
```

Restart Codex after installation so the new skill can be loaded.

## Example Prompt

```text
Use $marketing-copywriting to write a Xiaohongshu marketing post for my product.

Product:
We provide an enterprise AI employee infrastructure. Companies can connect once, let all employees use AI in a unified way, and keep billing, auditing, permission control, traceability, and reusable workflows.
```

## Notes

- Keep each skill in its own directory.
- Each skill should include a `SKILL.md` file with front matter.
- Supporting files, agent configs, templates, and images can live inside the same skill directory.
