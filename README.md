# grok-skills

A curated collection of **modular skills** for Grok and xAI agents.

Each skill is a self-contained, version-controlled package (`SKILL.md` + optional `scripts/`, `references/`, `assets/`) that specializes the agent for specific domains, workflows, or capabilities.

Skills follow the official [skill format](https://github.com/xai-org/grok-skills or internal docs) and can be easily added to any Grok environment.

## Why This Repo?

- **Reusability**: Battle-tested skills you can copy into your own `.grok/skills/` directory.
- **Version Control**: Track improvements, collaborate, and maintain history of prompt engineering and agent capabilities.
- **Discoverability**: A growing library of high-quality skills for research, creativity, coding, analysis, and more.
- **Standards**: Consistent structure and quality guidelines.

## Repository Structure

```
grok-skills/
├── README.md
├── skills/
│   ├── README.md                 # Skill index with descriptions & usage
│   ├── ai-usage-mastery/         # Prompt engineering, SOTA model strategies, Grok mastery
│   │   └── SKILL.md
│   ├── research-assistant/       # Deep web/X research, synthesis, fact-checking
│   │   └── SKILL.md
│   ├── image-prompt-expert/      # Advanced image generation & iterative editing
│   │   └── SKILL.md
│   └── code-architect/           # Software design, debugging, best practices
│       └── SKILL.md
├── templates/
│   └── new-skill-template.md     # Boilerplate for creating new skills
└── docs/
    └── creating-new-skills.md    # Guide + best practices
```

## Available Skills

| Skill                    | Description                                                                 | Best For                          |
|--------------------------|-----------------------------------------------------------------------------|-----------------------------------|
| **ai-usage-mastery**    | Comprehensive strategies for prompt engineering, CoT, few-shot, role prompting, Grok-specific real-time tool use, iteration, and multi-model workflows. | Leveling up AI prompting & usage |
| **research-assistant**  | Systematic research workflows: tool-triggered searches, multi-source synthesis, source evaluation, bias detection, and structured reporting. | Research, due diligence, analysis |
| **image-prompt-expert** | Crafting highly detailed, effective prompts for Grok Imagine and image editing. Includes iteration patterns and style references. | Visual content, storyboarding, design |
| **code-architect**      | Expert guidance on code architecture, debugging, refactoring, testing strategies, and clean code principles when collaborating with AI. | Software development & engineering |

## How to Use a Skill

1. Copy the desired skill folder (e.g. `skills/ai-usage-mastery/`) into your local Grok skills directory (usually `~/.grok/skills/` or equivalent in your environment).
2. The skill becomes available for the agent to load when relevant queries are made (or explicitly referenced).
3. Skills are designed to be **loaded on demand** and provide specialized instructions without bloating the base model context.

## How to Create a New Skill

1. Use the `skill-creator` skill or follow the template in `templates/new-skill-template.md`.
2. Create a new folder under `skills/<kebab-case-name>/`.
3. Write a high-quality `SKILL.md` following the frontmatter + imperative instructions format.
4. (Optional) Add `scripts/`, `references/`, or `assets/`.
5. Test thoroughly.
6. Submit a Pull Request with clear description of the skill's purpose and example use cases.

See `docs/creating-new-skills.md` for the full guide and quality checklist.

## Contributing

We welcome high-quality contributions!

- **Bug fixes / improvements** to existing skills: Open an issue or PR.
- **New skills**: Follow the template and contribution guidelines.
- Please keep skills focused, concise (< ~500 lines in SKILL.md), and genuinely useful (avoid duplicating base model knowledge).

## License

MIT License — feel free to use these skills in your own agents and projects.

---

*Maintained by the community and xAI enthusiasts. Built for maximum truth-seeking and capability extension.*