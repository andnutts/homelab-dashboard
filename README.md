# Homelab Dashboard

A modular, plugin-based management dashboard for Docker homelab environments.

## Features

- Plugin architecture with:
  - Categories
  - Versioning
  - Metadata validation
  - Hot reloading
  - Remote plugin repositories
- fzf-powered fuzzy menus
- ACME certificate browser
- Nginx Proxy Manager proxy host viewer
- Compose validator
- Network topology viewer
- Master compose health dashboard

## Directory Structure

core/       # dashboard engine
plugins/    # local plugins
repo/       # remote plugin repository (GitHub Pages)
docs/       # architecture and specifications

Code

## Installation

sudo cp core/homelab-dashboard /usr/local/bin/
sudo mkdir -p /usr/local/bin/homelab-dashboard.d
sudo cp plugins/*.plugin /usr/local/bin/homelab-dashboard.d/

Code

## Remote Plugin Repository

The `repo/` directory is designed to be served via GitHub Pages.

Your dashboard can install plugins with:

homelab-dashboard → Install Remote Plugin

Code

## License

MIT
