# README

Spoticloud-dl is a script to download playlists from either Spotify or Soundcloud with a max bandwidth of either 320kbps or 128kbps respectively. The script also appends metadata to the mp3s, including album art, artist and album name if applicable. 

## Installation

Use the pip to install requirements.txt

```bash
pip install requirements.txt
```

## Usage

Both a Spotify and Soundcloud API is neeed, blank key files are present within the repo.

For Spotify, create a new application within the Spotify developer tab to get a client_id, client_secret, redirect and a username

For Soundcloud, APIs have unfortunately disabled due to high demand, however you can still get a client_id and oaurth key from their main website:

Create a soundcloud account, login then head to soundcloud.com. Inspect element on the site then head to the network tab. There should be a domain along the lines of api-v2.soundcloud.com/me?client_id=xxxxxx, click on it and grab the client_id. Then go to headers and look for Authorization, your OAuth key should be there.
