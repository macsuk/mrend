# MRend :)

Turn Roblox models into clean, high quality icons

## ~> Tutorial

### 1. Install
~ Download and install the latest version of MRend.

### 2. Import FBX
~ Click **Import File** or drag your `.fbx` file into the app.  
~ Your model should load automatically ~> ready to render.  

### 3. Import Roblox Models
~ Open Roblox Studio and find your model in the **Explorer**.  
~ Right click the model ~> **Export Selection** ~> export it as an `.obj` file.  
~ Save the export into the `Export` folder inside your MRend directory.  
~ Your model should automatically appear in the export list.

> [!NOTE]
> If your model doesn't appear automatically ~> click **Load Export**.

## ~> Claude MCP Setup
~ If you want to use MRend with Claude via MCP, add the following to your MCP configuration:

```json
{
  "mcpServers": {
    "MRend": {
      "command": "node",
      "args": [
        "D:\\MRend\\mcp~server.js"
      ],
      "env": {
        "ICON_MAKER_EXE": "D:\\MRend\\MRend.exe"
      }
    }
  }
}
```

~> **Important:** Change `D:\\MRend\\` to your actual MRend installation path if it's different.
~> After that you must restart your claude fully.

## Claude Designs
~ Claude Designs will make claude adjust the rotation/zoom/lighting based on your game style.
~ If Claude Design is disabled he will ask you to rotate it and then chat will continue when you done.
