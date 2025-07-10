# A2A_MCP

A2A_MCP is a modular control platform designed for agent-based data processing and comparison. This project includes local and remote agents, a database, and demo scripts for comparing different agent approaches.

## Project Structure

- `a2a_mcp/`  
  Python virtual environment and dependencies.

- `adk-mcp/`  
  Main project code.
  - `demo_comparison/`  
    - `mcp_agent.py`: MCP agent implementation.
    - `traditional_agent.py`: Traditional agent implementation.
  - `local_mcp/`  
    - `agent.py`: Local agent logic.
    - `create_db.py`: Database setup script.
    - `server.py`: Local MCP server.
    - `prompt.py`: Prompt handling.
    - `database.db`: SQLite database.
    - `mcp_server_activity.log`: Server activity log.
  - `remote_mcp_agent/`  
    - `agent.py`: Remote agent logic.
    - `prompt.py`: Remote prompt handling.

## Setup

1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd A2A_MCP
   ```

2. Activate the Python virtual environment:
   ```bash
   source a2a_mcp/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r adk-mcp/requirements.txt
   ```

## Usage

- To run the local MCP server:
  ```bash
  python adk-mcp/local_mcp/server.py
  ```

- To run demo comparisons:
  ```bash
  python adk-mcp/demo_comparison/mcp_agent.py
  python adk-mcp/demo_comparison/traditional_agent.py
  ```

## License

Specify your license here.

## Contact

For questions or contributions, please open an issue or submit a pull request.