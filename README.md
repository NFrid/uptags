# Uptags - update your ID3 tags

Uptags is a somewhat simple python script that updates ID3 tags for mp3 files according to the file structure.

Usage:
`uptags *music dir*` (or w/out arguments to use default `~/Music`)

## Features

### File structure tags

`MUSIC_DIR/genre/artist/(album/)song`

### Album year

`year - album/`

### Song number

`number. song.mp3`

### Image cover (front)

the priority:
1. `number. song.jpg`
2. `song.jpg`
3. `number.jpg`
4. `_.jpg` (for a whole album)
4. `_.jpg` in an artist dir (for all his songs)

Note that you don't have to have proper file type (jpeg) or resolution of 600px or less with 1 by 1 ratio.
You just have to have any image file and name it like `*.jpg`.
The file will be automatically converted to proper format (**!!! it'll be overwritten !!!**)

## Things to do

- Year for a song in pattern `(year) title.mp3`
- File `*name*.txt` / `_.txt` where you can manually set tags for a song, an album, an artist, etc.
- Other music file formats (inc. `flac`)
- Configurable rules and patterns
- Configurable file structure
