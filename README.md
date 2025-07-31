# 📊 Anime OP/ED Dataset

A structured dataset of **Anime Openings (OP) and Endings (ED)** with YouTube metadata, covering the **top \~1000 anime** from MyAnimeList.
Each entry includes detailed song, artist, anime, and YouTube video information in JSON format.


## 📦 Dataset Overview

* **Anime Coverage** → \~1000 anime titles from MyAnimeList's top rankings.
* **Themes Covered** → All openings & endings for each anime (including multiple seasons / theme changes).
* **Data Source** → Combined from AnimeThemes.moe, public MyAnimeList data, and scraped YouTube metadata.
* **File Format** → JSON array.


## 📂 Example Entry

```json
{
  "query": "Haru (晴る) by Yorushika (ヨルシカ) Sousou no Frieren",
  "video_id": "CkvWJNt77mU",
  "title": "ヨルシカ - 晴る（OFFICIAL VIDEO）",
  "duration": 277.0,
  "view_count": 64052411,
  "channel": "ヨルシカ / n-buna Official",
  "url": "https://www.youtube.com/watch?v=CkvWJNt77mU",
  "thumbnails": [
    {
      "url": "https://i.ytimg.com/vi/CkvWJNt77mU/hq720.jpg",
      "height": 202,
      "width": 360
    }
  ],
  "anime": "Sousou no Frieren",
  "type": "opening",
  "type_number": "opening 2",
  "theme_number": 2,
  "original_theme_text": "2: \"Haru (晴る)\" by Yorushika (ヨルシカ) (eps 17-28)"
}
```


## 📑 Field Descriptions

| Field                     | Description                                                              |
| ------------------------- | ------------------------------------------------------------------------ |
| **query**                 | Search query used to find the YouTube video (song name + artist + anime) |
| **video\_id**             | YouTube video ID                                                         |
| **title**                 | Official video title from YouTube                                        |
| **duration**              | Video length in seconds                                                  |
| **view\_count**           | YouTube view count at time of scraping                                   |
| **channel**               | Name of the YouTube channel                                              |
| **url**                   | Full YouTube watch URL                                                   |
| **thumbnails**            | Array of available thumbnails (URL + dimensions)                         |
| **anime**                 | Anime title                                                              |
| **type**                  | `"opening"` or `"ending"`                                                |
| **type\_number**          | Theme type with number (e.g., `"opening 2"`)                             |
| **theme\_number**         | Numeric theme index                                                      |
| **original\_theme\_text** | Original source text from AnimeThemes/MyAnimeList                        |


## 🚀 Potential Uses

* **Anime music discovery**
* **Data analysis** (most viewed OP/EDs, trends over time)
* **Playlist generation** (YouTube, Spotify, etc.)
* **Anime recommendation systems**
* **Fan projects, dashboards, trivia bots**


## ⚠️ Disclaimer

* This dataset contains **links to publicly available YouTube videos** only.
* All video content belongs to their respective copyright owners.
* No videos are hosted in this repository.
* Data was collected from publicly accessible sources for research and non-commercial purposes.
* In **VERY** rare cases, the youtube data might be for another song with an identical title.
