# TikTok to YouTube Auto Poster

A Python script to automatically download videos from TikTok and upload them to YouTube. The script supports downloading TikTok videos by tag name or from a specific profile and handles errors during upload by restarting the process.

## Features

- **Download by Tag:** Fetch all TikTok videos related to a specific tag.
  ```
  python TiktokDownloader.py <tag_name>
  ```
  Example:
  ```
  python TiktokDownloader.py python
  ```

- **Download by Profile:** Download all videos from a specific TikTok profile.
  ```
  python TiktokDownloader.py <profile_url>
  ```
  Example:
  ```
  python TiktokDownloader.py https://www.tiktok.com/@think_now?_t=8sh89Xq3g0O
  ```

- **Error Handling:** Automatically restarts the upload process if errors occur, such as hitting YouTube's daily upload limit.

## Requirements

- Python 3.x
- Required Python libraries:
  - `requests`
  - `beautifulsoup4`
  - `google-api-python-client`
  - `google-auth`
  - `google-auth-oauthlib`
  - `google-auth-httplib2`

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/tiktok-youtube-autoposter.git
   cd tiktok-youtube-autoposter
   ```

2. Install the required libraries:
   ```
   pip install -r requirements.txt
   ```

3. Set up your Google API credentials for YouTube Data API.
   - Create a project in the [Google Cloud Console](https://console.cloud.google.com/).
   - Enable the YouTube Data API.
   - Download the OAuth 2.0 credentials JSON file and place it in the project directory.

## Usage

1. **Download by Tag:**
   ```
   python TiktokDownloader.py <tag_name>
   ```

2. **Download by Profile:**
   ```
   python TiktokDownloader.py <profile_url>
   ```

3. The script will automatically upload the videos to YouTube. If an error occurs during the upload, the script will restart the process.

## To-Do

- Improve error handling for YouTube API limits.
- Add support for scheduling uploads.
- Enhance logging and debugging features.

## Contributing

Feel free to fork the repository and submit pull requests to improve the script. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
