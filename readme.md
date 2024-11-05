# README

Spoticloud-dl is a script to download playlists from either Spotify or Soundcloud with a max bandwidth of either 320kbps or 128kbps respectively. The script also appends metadata to the mp3s, including album art, artist and album name if applicable. 

## Installation

Use the pip to install requirements.txt

```bash
pip install requirements.txt
```

## Preperation

Both a Spotify and Soundcloud API is needed, blank key files are present within the repo, remove the _temp extension to use within the script.

- **Spotify API setup:**

Spotify API credentials, create a new application within the Spotify developer tab to get a client_id, client_secret, redirect and a username

- **Soundcloud API setup:**

For Soundcloud, API apps have unfortunately been disabled due to high demand, however you can still get a client_id and OAuth key from their main website:

Create a soundcloud account, login then head to soundcloud.com. Inspect element on the site then head to the network tab. There should be a domain along the lines of api-v2.soundcloud.com/me?client_id=xxxxxx, click on it and grab the client_id. Then go to headers and look for Authorization, your OAuth key should be there.

### Example JSON for Spotify credentials

```json
{
    "username": "",
    "client_id": "",
    "client_secret": "",
    "redirect": ""
}
```

### Example JSON for Soundcloud credentials

```json
{
	"oauth": "", 
	"client_id": ""
}
```

## Usage

- **Download Spotify playlists:** Input a Spotify playlist URL, automatically downloads at 320kbps, metadata includes artist, album, genre, year of release and album art

- **Download Soundcloud playlists: Input a Soundcloud playlist URL, download at a max bitrate of 128kbps, metadata includes artist, and album art