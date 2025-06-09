# Record Prompts Rule

## Description
This rule records all user prompts and summaries of Amazon Q's actions to a markdown file at the root of the project.

## Instructions
After each interaction, append the user's prompt and a summary of your actions to the prompts.md file at the root of the project.

## Implementation
1. After processing each user request, create or append to the prompts.md file
2. Format each entry with:
   - Date and time of the prompt
   - The user's prompt (verbatim)
   - A brief summary of actions taken in response
3. Use markdown formatting for readability

## Example format to use
```markdown
## [Current Date and Time]

### Prompt
[User's prompt text]

### Actions
- [Summary of action 1]
- [Summary of action 2]
- [Summary of action n]

---
```

## Important
- Always append to the file, never overwrite existing content
- Keep summaries concise but informative
- Include all significant actions taken (files modified, commands executed, etc.)
- If the prompts.md file doesn't exist, create it