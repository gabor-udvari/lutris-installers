# Lutris Installers

The Lutris installers in this repository meet the following requirements:

- GOG.com games only, [FCKDRM](https://www.fckdrm.com/)
- The installer is running natively

## Innoextract

The scripts will display the progressbar of innoextract in a terminal. If Lutris will display a progress bar in the future, these will be replaced.

Execute task used as of now:

```
- execute:
    file: innoextract
    args: --gog --exclude-temp --progress --silent -d $GAMEDIR $setup
    description: Extracting game data...
```

Extract task planned for the future:

```
- extract:
    format: gog
    file: setup
    dst: $GAMEDIR
```
