# GrailPeople Beauty Advisor — Claude Skill

A Claude Code skill that turns Claude into a beauty shopping advisor backed by the [GrailPeople](https://grailpeople.com) database.

**Requires:** The [GrailPeople MCP connector](https://grailpeople.com/mcp) to be active in Claude.

## What it does

Routes beauty and skincare questions to the right GrailPeople tools in the right order — finding creator-backed product recommendations, brand reviews, and ingredient research. Includes citation format, honesty rules, zero-result retry logic, and response structure guidance.

## Example prompts

- "Best vitamin C serum according to dermatologists?"
- "Is CeraVe actually good or just overhyped?"
- "Show me what Hyram recommends for oily skin."
- "What are the best k-beauty moisturizers for sensitive skin?"

## Install

Add `SKILL.md` to your `.claude/skills/grailpeople-beauty-advisor/` directory.

## MCP connector

Connect GrailPeople at: `https://grailpeople.com/api/mcp` (no auth required)

Full docs: [grailpeople.com/mcp](https://grailpeople.com/mcp)
