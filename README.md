## Rojo Template
My personal template for Roblox Studio Projects I want to build using the Rojo plugin. The main thing for look out for here is the default.project.json file. 

The src folder hierarchy is based on the json file and the dummy scripts are just a personal preference, helps with my ocd when creating repos.

---

### default.project.json
```json
{
  "name": "Project Title",
  "tree": {
    "$className": "DataModel",

    "ReplicatedFirst": {
      "$path": "src/replicatedfirst"
    },

    "ReplicatedStorage": {
      "Shared": {
        "$path": "src/shared"
      },
      "Remotes": {
        "$path": "src/remotes"
      },
      "Packages": {
        "$path": "src/packages"
      }
    },

    "ServerScriptService": {
      "Server": {
        "$path": "src/server"
      }
    },

    "StarterGui": {
      "$path": "src/gui"
    },

    "StarterPlayer": {
      "StarterPlayerScripts": {
        "$path": "src/client"
      },
      "StarterCharacterScripts": {
        "$path": "src/character"
      }
    },

    "Lighting": {
      "$properties": {
        "Ambient": [0, 0, 0],
        "Brightness": 2,
        "GlobalShadows": true,
        "Technology": "ShadowMap"
      }
    }
  }
}
```

### Folder Hierarchy
Relevant to the Roblox Studio workspace.
```text
DataModel
├─ ReplicatedFirst
│  └─ src/replicatedfirst
├─ ReplicatedStorage
│  ├─ Shared
│  │  └─ src/shared
│  ├─ Remotes
│  │  └─ src/remotes
│  └─ Packages
│     └─ src/packages
├─ ServerScriptService
│  └─ Server
│     └─ src/server
├─ StarterGui
│  └─ src/gui
└─ StarterPlayer
   ├─ StarterPlayerScripts
   │  └─ src/client
   └─ StarterCharacterScripts
      └─ src/character
```