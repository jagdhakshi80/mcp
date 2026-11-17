# mcp
Step 1: Go to your project directory

bash
cd /Users//Documents/Repo/AIApps/MCP/mcptut
Step 2: Activate your environment

bash
source .venv/bin/activate
Step 3: Start the MCP Inspector
Run:


bash
uv run mcp dev server/weather.py
GitHub - modelcontextprotocol/inspector: Visual testing tool for MCP servers · GitHub
 
This starts the MCP development environment and opens the MCP Inspector in your browser.

Step 4: Test your tools
In MCP Inspector:

Open Tools.

Select get_alerts.

Enter these arguments:


json
{
  "state": "CA",
  "event_filter": "heat",
  "limit": 5,
  "include_expires": true
}
4. Click Run Tool.

You can also test ping without any arguments.

Step 5: Stop the server
When finished, return to Terminal and press:


text
Ctrl + C
Important: There are two different ways to run your MCP server:

Command

Purpose

uv run mcp dev server/weather.py

Development and testing with Inspector

uv run python server/weather.py

Run the server directly using stdio
 

 

