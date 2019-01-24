# spotify-data

[![License](https://img.shields.io/github/license/seankhliao/spotify-data.svg?style=for-the-badge)](githib.com/seankhliao/spotify-data)

Exploratory data analysis from Spotify's data export tool

## Data source

1. Button in web ui
   a. ~3 months of sparse data
2. Email support requesting more data
   a. ~6 months of more data
   b. still less than what other people got: [one](https://twitter.com/mikarv/status/1012386696934182912) and [two](https://twitter.com/steipete/status/1025024813889478656)

## Observations

- Lots of metadata
- Some data anonymization
- Opaque URIs for a lot of things
- 32 char track IDs dont match with 22 char IDs from web API
  - Example: idontwannabeyouanymore by Billie Eilish
    - 8443c4a5eb3b467bbb972ece90d86f8f
    - 41zXlQxzTi6cGAjpOXyLYH

## In this repo

`types.go` a file of mostly autogenerated, hand deduplicated Go types for the following files:

- `Download_.json`:
- `EndSong_.json`: Event when a track ends
- `Gaia_.json`:
- `Interaction_.json`: