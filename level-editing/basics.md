# Level editing - Basics

Level editing only supported on desktop currently. You will need a `coolfox.exe` and a `coolfox-x.x.x.jar`. The `exe` only helps to run the `java -jar coolfox-x.x.x.jar` command. The `jar` contains all the files needed to run the game. It is basically a zip file, you can unzip it with [7-Zip](https://www.7-zip.org/).

```{info}
The only important is the `data` folder for level editing. 
```

Extract it next to the `jar`, the important folders and files are the following:

```
data/
├── levels/
│   ├── objects/
│   │   └── *.png   
│   ├── world1/
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
└── scripts/
    ├── cutscenes/
    │   └── *.json   
    └── *.json  
```

* `levels`: contains the `tsx` files for the _Blocks_, _Objects_ and _Tilesets_ and the `tmx` files for the _Tilemaps_ and _Rules_. 
* `scripts`: contains the `json` files for the in-game cutscenes and scripts.