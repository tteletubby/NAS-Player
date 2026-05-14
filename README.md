# Audio Library Search

A lightweight single-file web interface designed for NAS servers and local directories. It transforms a standard directory listing into a searchable and mobile friendly music library without requiring a database or complex backend.

---

## Features

* **Zero Configuration**: Drop the file into any folder containing audio files and it works immediately.
* **Smart Search**: Real-time filtering for track names and file extensions.
* **Format Support**: Automatically detects and lists MP3, FLAC, WAV, OGG, M4A, OPUS and AIFF files.
* **Adaptive Design**: Separate layouts for desktop and mobile devices including a glassmorphism header.
* **No Dependencies**: Pure HTML, CSS and vanilla JavaScript with no external requests.

---

## Technical Details

The application works by fetching the local directory index and parsing anchor tags. It is ideal for low power hardware like Raspberry Pi or older NAS units because the client side handles all processing.

### Performance
* Minimal CPU usage on the server.
* Debounced search input to prevent interface lag.
* Hardware accelerated CSS animations for smooth scrolling.

---

## Installation

1. Download the search.html file.
2. Place it in the root of your music folder on your server.
3. Ensure your web server allows directory listings.
4. Access the file through your browser.

---

## Customization

The interface uses CSS variables for easy theming. You can modify the colors at the top of the file to match your setup:

```css
:root {
  --bg:      #0d0d0d;
  --surface: #161616;
  --accent:  #e8a045;
  --text:    #f0ebe3;
}
