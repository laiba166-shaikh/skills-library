---
name: text-improver
description: Transform raw, informal, or unstructured workplace text into clear, professional, and well-formatted written communication. Use when users need to polish, format, or professionalize any workplace writing including emails, project updates, requirements documents, design documents, meeting minutes, or deliverables summaries. Trigger on requests like "improve this text", "make this professional", "format this email", or when users provide raw text needing refinement.
---

# Text Improver

Transform raw workplace text into clear, professional communication while preserving original meaning and intent.

## Core Principles

- Preserve the original meaning exactly
- Improve sentence flow and grammar
- Remove unnecessary repetition
- Use clear headings, bullet points, and spacing
- Keep language professional and neutral
- Avoid emotional, casual, or conversational phrasing
- Avoid marketing language unless explicitly present
- Do not invent timelines, features, or decisions

## Required Inputs

1. **raw_text**: The original text to improve
2. **use_case**: One of: `email`, `project_update`, `requirements_document`, `design_document`, `meeting_minutes`, `deliverables_summary`
3. **tone**: One of: `formal`, `semi-formal`, `concise-professional` (default: `formal`)
4. **audience** (optional): Examples: `internal team`, `manager`, `client`, `stakeholders`, `technical team`

If use_case is unclear, ask for clarification before proceeding.

## Formatting by Use Case

### Email

- Add a clear subject line
- Start with a professional greeting
- Use short paragraphs
- End with a polite closing
- Do not include emojis
- Keep it scannable

Format:
```
Subject: [Subject Line]

[Greeting]

[Body with short paragraphs]

[Closing]
[Signature placeholder]
```

### Project Update

- Start with a short overview (1–2 lines)
- Use sections:
  - **Progress**: What has been completed
  - **Blockers**: Issues preventing progress (if any)
  - **Next Steps**: Upcoming actions
- Use bullet points
- Keep sentences brief and factual

### Requirements Document

- Use formal documentation style
- Include sections:
  - **Overview**: Purpose and context
  - **Functional Requirements**: Core capabilities (numbered list)
  - **Non-Functional Requirements**: Performance, security, etc. (if applicable)
  - **Assumptions / Constraints**: Known limitations or dependencies
- Use numbered lists for requirements
- Use precise, unambiguous language

### Design Document

- Use structured technical writing
- Include:
  - **Purpose**: Why this design exists
  - **Scope**: What is and isn't covered
  - **High-Level Design**: Architecture overview
  - **Key Components**: Major parts and their interactions
  - **Open Questions**: Unresolved items (if any)
- Avoid over-explaining
- Prefer clarity over verbosity

### Meeting Minutes

- Use clear headings:
  - **Meeting Details**: Date, time, purpose
  - **Attendees**: Who was present
  - **Discussion Summary**: Key points discussed
  - **Decisions**: Concrete decisions made
  - **Action Items**: Who is doing what
- Use bullet points
- Keep content factual and neutral
- Do not add opinions or interpretations

### Deliverables Summary

- List deliverables clearly
- Include:
  - Deliverable name
  - Status (if mentioned)
  - Brief description
- Use bullet or table-style formatting
- Keep language outcome-focused

## Output Rules

- Output only the final polished text
- Do NOT explain changes
- Do NOT mention the prompt or instructions
- Do NOT include analysis or commentary

## File Management

- If creating a file, save it in the `notes` directory
- Create the `notes` directory if it doesn't exist
- Use descriptive filenames that reflect the content type (e.g., `improved_requirements.md`, `email_draft.md`)
