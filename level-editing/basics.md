# Level editing - Basics

Level editing only supported on desktop currently. You will need a `coolfox.exe` and a `coolfox-x.x.x.jar`. The _JAR file_ contains all the files needed to run the game. It is basically a zip file, you can unzip it with [7-Zip](https://www.7-zip.org/).

Extract the `data` folder next to the `jar` file, the important folders and files are the following:

```
data/
├── levels/
│   ├── objects/
│   │   └── *.png   
│   ├── world1/
│   │   ├── level1.tmx
│   │   ├── level2.tmx
│   │   ├── levelN.tmx
│   │   ├── ...
│   │   ├── rule1.tmx   
│   │   ├── rule2.tmx   
│   │   ├── rule3.tmx   
│   │   └── rules.txt   
│   ├── world2/
│   │   └── ...   
│   ├── worldN/
│   │   └── ...   
│   ├── blocks.tsx
│   ├── objects.tsx
│   ├── tileset1.tsx
│   ├── tileset2.tsx
│   └── tilesetN.tsx
├── scripts/
│   ├── cutscenes/
│   │   └── *.json   
│   └── *.json
└── resources.json
```

* `levels`:  _Tileset_ `tsx`, _Tilemap_ `tmx` and _Rules_ `tmx` and `txt` files
  * `objects.tsx`: the _Objects_ that can be placed on the _Objects layer_.
  * `blocks.tsx`: the _Tiles_ that can be used on the _Blocks layer_.
  * `tilesetN.tsx`: the _Tiles_ that can be used for drawing on any other layer (no functionality).
  * `rule1.tmx`: Rules for automapping the _Ground layer_
  * `rule2.tmx`: Rules for automapping the _Grass layer_
  * `rule3.tmx`: Rules for automapping the _Water layer_
  * `rules.txt`: List of the rules that will be applied on `Ctrl + M` (automapping)


* `scripts`: contains the `json` files for the cutscene scripts and scripts that run in-game.
  * `cutscenes`: contains the cutscene scripts, this folder is only for separation from the in-game scripts.


* `resources.json`: this file contains all the information about the resources used in the game in _JSON format_, like worlds, levels, textures, sounds, etc.