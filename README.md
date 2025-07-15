# YouTube Channel Test Automation

This project demonstrates automated testing of YouTube using Playwright Model Context Protocol (MCP). The test suite automates user interactions with YouTube's interface and generates detailed HTML reports.

## Project Structure

```
MCP/
├── .vscode/
│   ├── mcp.json        # MCP configuration
│   └── settings.json   # VS Code settings
├── prompt/
│   └── prompt.md       # Test specifications
├── test_report.html    # Generated test report
└── README.md          # This file
```

## Test Scenario

The automated test performs the following steps:
1. Navigates to YouTube homepage
2. Searches for "Errors Overflow"
3. Verifies search results and clicks on the first channel
4. Generates an HTML report with test results

## Prerequisites

- Visual Studio Code
- Node.js
- Playwright MCP Server (@executeautomation/playwright-mcp-server)

## Configuration

The project uses MCP (Model Context Protocol) for test automation. The configuration is defined in `.vscode/mcp.json`:

```json
{
  "servers": {
    "playwright": {
      "command": "npx",
      "args": ["-y", "@executeautomation/playwright-mcp-server"]
    }
  }
}
```

## Test Report

The automation generates an HTML report (`test_report.html`) that includes:
- Detailed step-by-step execution results
- Expected vs. actual outcomes
- Test execution summary

## Screenshots

Screenshots are automatically captured during test execution and saved in the working directory. The latest test execution screenshot is referenced in the HTML report.

## Customization

Test scenarios can be modified by updating the `prompt.md` file in the `prompt` directory. The file follows a structured format:
- Website URL
- Step-by-step instructions
- Expected outcomes for each step
- Report format specification
