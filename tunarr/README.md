# Tunarr – Home Assistant Add-on

![Tunarr Logo](icon.png)

> **Disclaimer:** This add-on is not affiliated with, endorsed by, or in any way officially connected to the [Tunarr](https://github.com/chrisbenincasa/tunarr) project or its authors.

## About

[Tunarr](https://github.com/chrisbenincasa/tunarr) lets you turn your local media library into full-fledged IPTV channels. You can create custom channels from your Plex, Jellyfin, or Emby libraries and stream them to any IPTV-compatible player, including Plex DVR, Jellyfin Live TV, and more.

This add-on runs Tunarr directly inside Home Assistant OS, built from the official Docker image published by the Tunarr project (`chrisbenincasa/tunarr` on Docker Hub).

## Installation

1. In Home Assistant, navigate to **Settings → Add-ons → Add-on Store**.
2. Click the **⋮ menu** (top-right) and choose **Repositories**.
3. Add the following URL and click **Add**:
   ```
   https://github.com/Thepowa753/hassio_tunarr
   ```
4. Find the **Tunarr** add-on in the store and click **Install**.
5. Optionally adjust the **Web port** (default: `8000`) in the *Network* tab.
6. Click **Start**.
7. Open the **Web UI** tab or navigate to `http://<your-ha-ip>:8000` to access Tunarr.

## Configuration

| Option | Description |
|--------|-------------|
| **Port** (Network tab) | The port Tunarr will listen on. Default is `8000`. |

Tunarr stores its configuration and database inside the add-on's `/config` folder (mapped to the Home Assistant `config` volume).

## Usage

After the first start, Tunarr will guide you through a setup wizard where you can:

- Connect your Plex, Jellyfin, or Emby media server
- Create IPTV channels from your media library
- Configure the XMLTV guide data URL for use with Jellyfin Live TV, Plex DVR, etc.

The web interface is available at `http://<your-ha-ip>:8000`.

## Support

For issues related to this **Home Assistant add-on**, open an issue at:
<https://github.com/Thepowa753/hassio_tunarr/issues>

For issues with **Tunarr itself**, please use the upstream project:
<https://github.com/chrisbenincasa/tunarr/issues>
