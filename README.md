\# Prompt Suppressor (MCP)



A standalone MCP server that enforces clean prompt structure, strips model‑invented instructions, and detects capability hallucinations before they propagate through your system.



This repository contains the full implementation and runs independently. It does not depend on the full suite.



\## Usage



Add this server to your Claude Desktop or MCP client configuration:



{

&nbsp; "mcpServers": {

&nbsp;   "prompt\_suppressor": {

&nbsp;     "command": "python3",

&nbsp;     "args": \["/path/to/mcp-prompt-suppressor/server.py"]

&nbsp;   }

&nbsp; }

}



\## What it does



\- Removes model‑invented system instructions  

\- Normalises prompt structure  

\- Detects capability hallucinations  

\- Flags unsafe or structurally invalid prompt patterns  



\## Relationship to the full suite



This suppressor is also included in the consolidated mcp-hallucination-suite, which bundles all four suppressors and provides a meta-orchestrator:



https://github.com/steveswain14/mcp-hallucination-suite

