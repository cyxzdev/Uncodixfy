# Uncodixify

<p align="center">
  <img src="images/thumb.jpg" alt="Uncodixify" width="100%">
</p>


GPT is surprisingly bad at UI design.

If you ask it to generate interfaces long enough, you start noticing the same bad design-patterns repeating.

Floating cards.  
Oversized rounded corners.  
Gradient-heavy dashboards.    
Decorative labels everywhere.  
Glass panels.  


After a while you can recognize a “GPT UI” immediately.

This file exists to stop that.

---

## What this is

`uncodixify.md` is a rule set that forces GPT to stop relying on its usual UI habits.

Instead of letting it improvise design decisions, the file blocks the patterns it almost always falls back to and pushes it toward more normal interfaces.

It doesn't try to teach GPT how to design.

It mostly just tells it what **not** to do.




## Using it

Include `uncodixify.md` in your prompt or system instructions when asking GPT to generate UI.

Example:
<p align="center">
  <img src="images/1.png" width="48%">
  <img src="images/2.png" width="48%">
</p>

Before (Typical GPT UI) | After (Uncodixified)

<p align="center">
  <img src="images/4.png" width="48%">
  <img src="images/3.png" width="48%">
</p>

Before (Typical GPT UI) | After (Uncodixified)

---
## Agent Skill

Uncodixfy is also available as an agent skill via SKILL.md. This works with any AI coding agent that supports the skill format (Claude Code, etc.).

### Windows (PowerShell)

```powershell
git clone https://github.com/cyxzdev/Uncodixfy.git "$HOME\.claude\skills\uncodixfy"
```

### macOS

```bash
git clone https://github.com/cyxzdev/Uncodixfy.git ~/.claude/skills/uncodixfy
```

### Linux

```bash
git clone https://github.com/cyxzdev/Uncodixfy.git ~/.claude/skills/uncodixfy
```

Once installed, invoke it with:

```text
/uncodixfy
```
