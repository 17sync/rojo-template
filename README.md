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
      "$path": "src/replicatedstorage"
    },

    "ServerScriptService": {
      "$path": "src/serverscriptservice"
    },

    "ServerStorage": {
      "$path": "src/serverstorage"
    },

    "StarterGui": {
      "$path": "src/startergui"
    },

    "StarterPlayer": {
      "StarterPlayerScripts": {
      "$path": "src/starterplayerscripts"
      },

      "StarterCharacterScripts": {
      "$path": "src/startercharacterscripts"
      }
    },
    
    "SoundService": {
      "$path": "src/soundservice"
    },

    "TextChatService": {
      "$path": "src/textchatservice"
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
│  │  └─ src/replicatedstorage/shared
│  ├─ Remotes
│  │  └─ src/replicatedstorage/remotes
│  ├─ Assets
│  │  └─ src/replicatedstorage/assets
│  └─ Packages
│      └─src/replicatedstorage/packages  
├─ ServerScriptService
│  └─ Services
│     └─ src/serverscriptservice/services
├─ ServerStorage
├─ StarterGui
│  └─ src/startergui
├─ StarterPlayer
│  ├─ StarterPlayerScripts
│  │  └─ src/starerplayerscripts
│  └─ StarterCharacterScripts
│     └─ src/startercharacterscripts
├─ SoundService
│   └─ src/soundservice
└─ TextChatService
```