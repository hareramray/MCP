# Playwright MCP Prompt

## Instructions

1. **Enter the website URL** you want to test.
2. **Provide step-by-step instructions** for the actions to perform (e.g., "Go to homepage", "Click login", "Enter username and password", "Verify dashboard loads").
3. **Specify expected outcomes** for each step.
4. **Choose report format** (e.g., HTML, JSON, Markdown).

## Now this is Prompt

```
Website: https://www.youtube.com/

Steps:
1. Navigate to https://www.youtube.com/
    - Expect: Homepage loads 
2. Search for "Errors Overflow" in search bar
    - Expect: Redirects to https://www.youtube.com/results?search_query=Errors+Overflow
3. Verify the page contains the text "Errors Overflow". Click on the Errors overflow first youtube channel
    - Expect: Text is visible on the page
close the chromium browser
Report format: HTML
save report in the working directory
```

## Output

- Playwright will execute the steps.
- A report will be generated in the chosen format, summarizing actions, results, and any errors.
