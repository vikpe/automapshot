# automapshot

> Automate screenshots of QuakeWorld maps.

Uses an ezQuake client to cycle through maps, load camera settings and then take screenshots.

## Requirements

* Unix build of [ezQuake](https://github.com/ezQuake/ezquake-source)
* `.env` (copy `.env.example` and set values)
* `map_settings.json` - Settings per map

## Usage

```shell
automapshot [<maps> ...]
```

### Specific maps

```shell
automapshot dm2
automapshot dm2 dm4 dm6
```

### All maps

Create mapshot for all maps defined in `map_settings.json`.

```shell
automapshot all
```

## How to create thumbnails

```shell
 mkdir thumbs
 mogrify  -format jpg -path thumbs -thumbnail 400x300 *.jpg
 ```

## Related projects

* [QuakeWorld Mapshots](https://github.com/vikpe/qw-mapshots)
* [QuakeWorld Hub](https://github.com/quakeworldnu/hub.quakeworld.nu) 
