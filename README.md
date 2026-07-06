## Rojo Template
My personal template for Roblox Studio Projects I want to build using the Rojo plugin. The main thing for look out for here is the default.project.json file. 

The src folder hierarchy is based on the json file and the dummy scripts are just a personal preference, helps with my ocd when creating repos.

---

### default.project.json
```json
{
  "name": "Project Template",
  "tree": {
    "$className": "DataModel",

    "ReplicatedFirst": {
      "$path": "src/replicatedfirst"
    },

    "ReplicatedStorage": {
      "$path": "src/replicatedstorage",

      "Shared": {
        "$path": "src/replicatedstorage/shared"
      },
      "Remotes": {
        "$path": "src/replicatedstorage/remotes"
      },
      "Assets": {
        "$path": "src/replicatedstorage/assets",

        "Animations": {
          "$path": "src/replicatedstorage/assets/animations"
        },
        "Sounds": {
          "$path": "src/replicatedstorage/assets/sounds"
        },
        "Effects": {
          "$path": "src/replicatedstorage/assets/effects"
        },
        "Models": {
          "$path": "src/replicatedstorage/assets/models"
        },
        "Packages": {
          "$path": "src/replicatedstorage/packages"
        }
      }
    },

    "ServerScriptService": {
      "$path": "src/serverscriptservice",

      "Services": {
        "$path": "src/serverscriptservice/services"
      }
    },

    "StarterGui": {
      "$path": "src/startergui"
    },

    "StarterPlayer": {
      "$path": "src/starterplayer",

      "StarterPlayerScripts": {
        "$path": "src/starterplayer/starterplayerscripts"
      },
      "StarterCharacterScripts": {
        "$path": "src/starterplayer/startercharacterscripts"
      }
    },

     "SoundService": {
            "$path": "src/soundservice"
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
      └─src/replicatedstorage/packages  
├─ ServerScriptService
│  └─ Services
│     └─ src/serverscriptservice/services
├─ StarterGui
│  └─ src/startergui
├─ StarterPlayer
│  ├─ StarterPlayerScripts
│  │  └─ src/starerplayerscripts
│  └─ StarterCharacterScripts
│     └─ src/startercharacterscripts
└─ SoundService
    └─ src/soundservice
```