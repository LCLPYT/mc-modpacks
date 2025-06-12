# mc-modpacks
Available modpacks:

| Modpack              | Loader | 1.21.4 | 1.21.5 |
|--------------------- |--------|--------|--------|
| LCLP's MiniGame Pack | Fabric | ✅     | ✅     |
| Builder Utils        | Fabric | ✅     | ✅     |
| Survival Pack        | Fabric | ❌     | ✅     |

## Manage and maintain modpacks
This project uses [Packwiz](https://packwiz.infra.link/) to manage the modpacks.

### Add a mod from Modrinth
```bash
packwiz modrinth add sodium
```

### Add a mod from GitHub
```bash
packwiz github add LCLPYT/mc-option-sync

# or use full url
packwiz github add https://github.com/LCLPYT/mc-option-sync
```

### Add a mod from some direct download URL
```bash
packwiz url add <mod id> <direct url>
```

### Adding local files
Just add any files to the modpack directory, as if it was the minecraft directory. Then refresh the index:
```bash
packwiz refresh
```

Files that should not be included in the modpack can be put in the `.packwizignore` file.

### Exporting the modpack
You can export a modpack as `.mrpack` file:
```bash
packwiz modrinth export
```

### Migrating to another Minecraft version
```
packwiz migrate minecraft <version>
```
