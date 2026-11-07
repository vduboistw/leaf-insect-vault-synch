# Markdown Generation Standard

Unless explicitly requested otherwise, all generated `.md` files shall use standard GitHub-Flavored Markdown (GFM), compatible with Obsidian, GitHub, VS Code, Typora and most Markdown editors.

## General

- UTF-8 encoding.
- Unix (LF) line endings preferred.
- Plain text only.
- No hidden formatting.
- No HTML unless specifically requested.
- No Markdown dialects requiring special parsers.
- Output proposed as both a downloadable file link and an output in a text box in the UI

## Headings

- Use ATX headings (`#`, `##`, `###`).
- Leave one blank line before and after headings.
- Do not skip heading levels unnecessarily.

## Tables

Use standard pipe tables only.

Example:

| Column A | Column B |
|----------|----------|
| A        | B        |

Rules:

- Header separator row is mandatory.
- One physical line per table row.
- No wrapped rows.
- No multiline cells.
- No merged cells.
- Keep columns aligned with spaces where practical for readability.

## Lists

- Use `-` for unordered lists.
- Use `1.` for ordered lists.
- Indent nested lists with four spaces.

## Code

- Fence code blocks using triple backticks.
- Specify language whenever known.

Example:

```python
print("Hello")
```

## Emphasis

Use only:

- *italic*
- **bold**
- `inline code`

Avoid nested emphasis unless necessary.

## Links

Use standard Markdown links:

[Title](URL)

## Images

Use standard syntax:

![Alt text](image.png)

## Horizontal rules

Use:

---

## Tables intended as databases

When a table is intended to be maintained over time:

- Never reorder rows unless requested.
- Never silently rename columns.
- Preserve all existing columns.
- Append rather than rewrite when possible.
- Preserve exact wording unless correction is explicitly requested.

## File updates

When asked to update an existing Markdown file:

1. Read the entire document.
2. Preserve all information.
3. Modify only what is requested.
4. Refresh the “update date” when mentioned
5. Add new information in relevant sections, without duplication of sections
6. Never compress or summarize existing content.
7. Return a complete replacement file.

## Compatibility goal

Generated Markdown should render correctly without modification in:

- Obsidian
- GitHub
- GitLab
- VS Code Markdown Preview
- Typora
- MarkText

## Canonical project files

Some Markdown files act as living project databases.

These files are authoritative records rather than prose.

When updating them:

- Preserve ordering unless instructed otherwise.
- Preserve comments and notes.
- Preserve blank lines separating logical sections.
- Never delete historical information.
- Prefer appending over rewriting.
- If information is uncertain, mark it as uncertain rather than replacing existing data.
- Keep the original document structure - the “append only” rule means that existing notes, records and entries are preserved, and new notes, records and entries are added within the existing body of the document. 
- Generate the complete updated file, not a patch.