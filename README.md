# YouTube Playlist Downloader using Electron and yt-dlp

This application is a desktop program built using **Electron** and **JavaScript** with a user interface designed with **Tailwind CSS**. The project aims to download YouTube playlists using the **yt-dlp.exe** tool, with support for specifying the start and end points of the playlist to download, or downloading the entire playlist.

---

## Introduction

The application relies on a modern, user-friendly interface along with backend logic that executes yt-dlp.exe via Node.js. It allows users to enter a YouTube playlist URL and specify start and end values to download a specific set of videos or all the videos in the playlist.

---

## Main Features

- **Attractive and User-Friendly Interface:** The interface, designed using Tailwind CSS, ensures a smooth user experience.
- **Playlist Downloading:** Users can input a YouTube playlist URL with the option to set a starting point (for example, beginning from video number 400) or download the entire playlist.
- **Download Customization Options:** Supports selecting video quality and choosing a file-naming template that includes the video index and title.
- **Executing yt-dlp.exe from the Application:** Utilizes Node.js to call yt-dlp.exe with the proper parameters and receives process output to display progress and results.
- **Real-Time Output Updates:** Displays information related to download progress and error messages directly in the interface.
- **Windows Compatibility:** Designed to leverage yt-dlp.exe, with the possibility of adaptation for other systems by providing the appropriate version.

---

## Tools and Technologies Used

- **Electron:** A framework for developing desktop applications using web technologies.  
  For more details, see: [Electron Documentation](https://www.electronjs.org/docs/latest) :contentReference[oaicite:0]{index=0}

- **JavaScript:** The primary language used for developing the application logic and managing backend processes.

- **Tailwind CSS:** A CSS library based on the utility-first methodology for designing modern and responsive user interfaces.  
  For more information, see: [Tailwind CSS Documentation](https://tailwindcss.com/docs) :contentReference[oaicite:1]{index=1}

- **yt-dlp.exe:** An advanced tool for downloading videos and playlists from YouTube, an updated fork of youtube-dl.  
  For further details, see: [yt-dlp GitHub](https://github.com/yt-dlp/yt-dlp) :contentReference[oaicite:2]{index=2}

- **Node.js:** A JavaScript runtime used to execute external commands and run yt-dlp.exe.

---

## Overall Project Structure

The project consists of several key components:
- **Main Process:** The Electron application startup file that initializes the app and creates the application window.
- **Renderer Process (User Interface):** The HTML file containing the UI design using Tailwind CSS, along with a JavaScript file that handles user interactions.
- **Configuration File (package.json):** Contains project settings and the scripts required to run the application.
- **yt-dlp.exe Tool:** This file is included in the project folder to facilitate its execution and to run download commands.

---

## How the Application Works

1. **User Input:**  
   The user enters a YouTube playlist URL with the option to specify a starting point (such as beginning the download from video number 400) or selecting a particular range to download a specific set of videos, or leaving the options open to download the entire playlist.

2. **Executing the Download Command:**  
   The application prepares the necessary parameters (such as selecting video quality with the -f parameter and choosing a file naming template with -o) and then calls yt-dlp.exe via Node.js to carry out the download process.

3. **Running yt-dlp.exe:**  
   The specified parameters are passed to the tool to download the videos according to the chosen options, with the process output (download progress or error messages) updated and displayed directly in the application interface.

4. **Displaying Results:**  
   During the download, yt-dlp outputs (both progress information and error messages) are shown in a dedicated area in the application, allowing the user to monitor the process.

5. **Download Options:**  
   The application allows the user to download either a specific portion of the playlist or the entire playlist, thus providing greater flexibility in the downloading process.

---

## Setup and Execution Steps

- **System Requirements:**  
  Node.js must be installed on the device, and yt-dlp.exe must be downloaded and placed within the project folder.

- **Project Initialization:**  
  Set up the core files (such as the main Electron application file, the user interface HTML file, and the package.json configuration file) according to the structure described above.

- **Running the Application:**  
  After completing the necessary setup and adjusting the options as needed, the application can be run with Electron commands to display the user interface for entering the playlist URL and download options.

---

## References

- **Electron Documentation:**  
  [https://www.electronjs.org/docs/latest](https://www.electronjs.org/docs/latest) :contentReference[oaicite:3]{index=3}

- **Tailwind CSS Documentation:**  
  [https://tailwindcss.com/docs](https://tailwindcss.com/docs) :contentReference[oaicite:4]{index=4}

- **yt-dlp GitHub:**  
  [https://github.com/yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) :contentReference[oaicite:5]{index=5}
