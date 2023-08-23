Certainly! Here's a comprehensive `README.md` for your project:

---

# E621 Pool Downloader

A simple Python script to download image pools from e621.net.

## Features

- Downloads all images from a specified pool.
- Organizes downloaded images into folders named after the pool ID and pool name.
- Renames images based on their order in the pool, with the last image being the first page and the first image being the last page.
- Creates a `.nfo` file for each image containing metadata such as artist, tags, description, and sources.

## Prerequisites

- Python 3.x
- `requests` library

## Setup

1. Clone the repository or download the `index.py` script.
2. Install the required libraries:

```bash
pip install requests
```

3. Change the usename and APIKey in the base64.b64encode line 

```json
    "Authorization": "Basic " + base64.b64encode("username:APIKey".encode()).decode() #remeber to add username and APIKey to this line
```

Replace `YourE621Username` and `YourE621APIKey` with your e621 username and API key respectively.

4. Create a `pools.txt` file in the same directory as the script. Each line in this file should contain a pool ID that you want to download.

## Usage

Run the script:

```bash
python index.py
```

The script will download all images from the pools specified in `pools.txt` and organize them into the `downloads` directory.

## Notes

- Ensure you have the necessary permissions to download content from e621.net.
- Respect the terms of service of e621.net and use this script responsibly.

## License

This project is open-source and available under the MIT License.

---

Feel free to modify or expand upon this README as needed for your project!
