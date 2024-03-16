# Sublime_setting
My sublime package list and settings

## Package list
1. BracketHighlight
2. FileIcons
3. LSP
4. LSP-pyright
5. Package Control
6. python-black
7. Terminal
8. Terminus

## Settings
1. Keymap
```
[
    { 
        "keys": ["alt+1"], "command": "toggle_terminus_panel"
    },

    { 
        "keys": ["alt+2"], "command": "terminus_open"
    },

    { 
        "keys": ["ctrl+alt+1"], "command": "terminus_open", "args": {
            "cmd": "ipython",
            "cwd": "${file_path:${folder}}"
        }
    },
    
    {
        "keys": ["ctrl+1"], "command": "open_terminal_project_folder"
    },
]

```

2. Terminal
```
{
	
  "terminal": ${path},
  "parameters": ["."]

}
```

3. Terminus
```
{
    "default_config": {
        "linux": null,    // login shell
        "osx": Zsh,      // login shell
        "windows": "PowerShell",
    },

    "view_settings": {
        "font_face": "JetBrainsMono NF",
        "font_size": 10,
    },

    "theme": "default",
}

```

4. Pyright
```
// Settings in here override those in "LSP-pyright/LSP-pyright.sublime-settings"

{
	"settings": {
		"python.pythonPath": ${python}
	}
}
```
