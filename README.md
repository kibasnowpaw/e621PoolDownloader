# e621 Downloader

This script is designed to download image posts from specified pools on e621 and organize them into directories named after the artist and pool. Additionally, it creates `.nfo` files in XML format for each downloaded post, containing relevant metadata.

## Features

- Downloads posts from specified pools on e621.
- Organizes downloaded posts into directories named in the format `[Artist Name] Pool Name`.
- Generates `.nfo` files in XML format for each post with metadata such as title, artist, tags, description, and sources.
- Sanitizes directory names to ensure they are valid and free from unwanted characters.
- Skips downloading files that already exist in the target directory.
- Uses BeautifulSoup to extract tags from the gallery page.

## Requirements

- Python 3.x
- `requests` library
- `BeautifulSoup` library
- `xml.etree.ElementTree` module

## Setup

1. Ensure you have Python 3.x installed.
2. Install the required libraries:
   ```
   pip install requests beautifulsoup4
   ```
3. Clone this repository or download the script.
4. Update the `HEADERS` constant in the script with your e621 username and API key.
5. Create a `pools.txt` file in the same directory as the script. Each line in this file should contain a pool ID from e621 that you wish to download.

## Usage

Run the script:
```
python script_name.py
```
Replace `script_name.py` with the name you've saved the script as.

The script will download the posts from the specified pools and organize them into directories within a `downloads` folder. Each post will also have an associated `.nfo` file containing its metadata.

## Notes

- Ensure you have the necessary permissions to access and download content from e621.
- Respect the terms of service and usage guidelines of e621 when using this script.
