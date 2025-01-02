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
  python TiktokDownloader.py https://www.tiktok.com/@think_now
  ```

- **Error Handling:** Automatically restarts the upload process if errors occur, such as hitting YouTube's daily upload limit.but need to fix on other error you need to keep an eye

## Requirements

- Python 3.x
- Required Python libraries:
  - `requests`
  - `beautifulsoup4`
  - `selenium`
  - `tqdm`


## Installation

1. Clone the repository:
   ```
     Download zip file from here 
      then run "chromefix.cmd"
      login to your youtube and tiktok account and close the browser
   then edit "tiktok tags.cmd"
    change tag or past url like 
    then it work on its self , next time you want to run again then open "Start.cmd"
   ```



3. The script will automatically upload the videos to YouTube. If an error occurs during the upload, the script will restart the process.

## To-Do

- Improve error handling for YouTube upload section.
- Add support for scheduling uploads.
- Enhance logging and debugging features.

## Contributing

Feel free to fork the repository and submit pull requests to improve the script. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
