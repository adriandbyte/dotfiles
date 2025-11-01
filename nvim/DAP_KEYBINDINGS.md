# DAP (Debug Adapter Protocol) Keybindings

## Breakpoints
- `<leader>db` - Toggle Breakpoint
- `<leader>dB` - Set Conditional Breakpoint (prompts for condition)

## Debug Controls
- `<leader>dc` - Continue (start/resume debugging)
- `<leader>di` - Step Into
- `<leader>do` - Step Out
- `<leader>dO` - Step Over
- `<leader>dt` - Terminate (stop debugging)

## UI
- `<leader>du` - Toggle DAP UI
- `<leader>de` - Eval (evaluate expression under cursor or selection)

## Debug Configurations

### Available Launch Configurations
The following configurations are loaded from `.vscode/launch.json` in your workspace:

1. **Run Script: develop** (node-terminal)
   - Command: `yarn run develop`

2. **Debug Strapi (UTC)** (node)
   - Debugs Strapi in development mode
   - Sets timezone to UTC
   - Args: `develop`

### Fallback Configurations (JavaScript/TypeScript)
If no launch.json is present, these configurations are available:

1. **Launch file** - Debug current file
2. **Attach** - Attach to running Node.js process

## Breakpoint Signs
- `●` - Regular breakpoint
- `◆` - Conditional breakpoint / Log point
- `→` - Current execution line (stopped)
- `` - Rejected breakpoint

## DAP UI Features
When debugging starts, the DAP UI opens automatically with:
- Variables view
- Watch expressions
- Call stack
- Breakpoints list
- Console output

The UI closes automatically when debugging terminates or exits.
