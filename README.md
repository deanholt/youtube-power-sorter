# YouTube Playlist Power Sorter & Player

A client-side web application that bypasses YouTube's native limitations, allowing you to instantly sort and seamlessly play massive YouTube playlists by view count, duration, and more.

## 💡 The Origin Story

This project was born out of frustration with the official Eurovision Song Contest playlist. I was staring at a list of 35 videos, able to see all the individual view counts, but manually scanning up and down the list to figure out which performance was the next most popular was an unnecessary challenge. 

I realized this was a UX failure that could be simply fixed with a custom HTML wrapper. What started as a quick script to sort view counts evolved into a full-featured, auto-advancing media player.

## ✨ Features

* **Advanced Sorting Algorithms:** Sort any public YouTube playlist by:
  * **View Count** (Find the hidden gems or the viral hits)
  * **Duration** (Shortest to longest, or vice versa)
  * **Date Added** (Chronological viewing)
  * **Title & Channel Name** (A-Z alphabetical grouping)
* **Integrated Auto-Player:** Uses the YouTube IFrame API to automatically advance to the next video in your *newly sorted* list when the current one finishes.
* **Active State Tracking:** Never lose your place. The sidebar automatically highlights and scrolls to the currently playing video.
* **100% Client-Side:** No backend servers, no databases, and no stored user data. It runs entirely in your browser.

## 🛠️ Tech Stack

* HTML5 / CSS3
* Vanilla JavaScript (ES6+)
* [YouTube Data API v3](https://developers.google.com/youtube/v3)
* [YouTube IFrame Player API](https://developers.google.com/youtube/iframe_api_reference)

## 🚀 How to Use It

Because this app communicates directly with YouTube's database, it requires a free YouTube Data API key to function. 

### Option 1: Live Demo (BYOK - Bring Your Own Key)
👉 **[Try the Live Demo Here](https://deanholt.github.io/youtube-power-sorter/)**

1. Navigate to the live link.
2. Paste your free Google Cloud API Key into the top box.
3. Paste any public YouTube Playlist URL.
4. Click **Load Playlist**.

### Option 2: Run Locally
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/deanholt/youtube-playlist-power-sorter.git
   ```

2.  Open the project folder in your preferred code editor (like VS Code).
3.  If you are using VS Code, install the **Live Server** extension.
4.  Open `index.html` and click **Go Live** in the bottom right corner of your editor.
5.  Provide your API key and playlist URL in the browser window.

## 🔑 Getting an API Key

If you don't have a YouTube Data API v3 key, you can get one for free:

1.  Go to the [Google Cloud Console](https://console.cloud.google.com/).
2.  Create a new project.
3.  Navigate to **APIs & Services \> Library**.
4.  Search for **YouTube Data API v3** and click **Enable**.
5.  Navigate to **Credentials**, click **Create Credentials**, and select **API Key**.

## 📖 Release History

  * **v1.0.0:** Official stable release.
  * **v0.4.x:** Introduced comprehensive multi-property sorting (Date, Duration, Title, Channel) and robust duration parsing.
  * **v0.3.x:** Completely overhauled UI to a modern dark-mode layout and integrated asynchronous API loading for stable playback.
  * **v0.2.x:** Integrated the native YouTube IFrame player for seamless, in-app viewing.
  * **v0.1.0:** Initial proof-of-concept.

## 📝 License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).