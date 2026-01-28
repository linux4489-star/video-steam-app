# 🎬 MovieHub - Video Streaming Website

A complete video streaming platform with upload, playback, and mobile support. Perfect for hosting and streaming full movies.

## Features ✨

- **📺 Video Upload**: Upload full movies up to 5GB
- **▶️ Video Playback**: Smooth streaming with HTML5 video player
- **📱 Mobile Responsive**: Perfect on desktop, tablet, and mobile devices
- **🔍 Search**: Find movies quickly with search functionality
- **📚 Library**: Manage your uploaded videos
- **🎨 Modern UI**: Beautiful, intuitive interface
- **⚡ Fast Streaming**: Supports video range requests for smooth playback
- **🗑️ Delete Videos**: Remove videos from your library

## Supported Video Formats

- MP4 (H.264)
- WebM
- AVI
- MOV (QuickTime)
- FLV
- X-MSVIDEO

## System Requirements

- Node.js 14+ 
- npm or yarn
- 10GB+ disk space for videos
- Modern web browser (Chrome, Firefox, Safari, Edge)

## Installation
# MovieHub - READY TO DEPLOY EVERYWHERE
### 1. Install Dependencies

```bash
cd video-streaming-app
npm install
```

### 2. Start the Server

```bash
```

Or for development with auto-reload:

```bash
npm run dev
```
### 3. Open in Browser

Navigate to `http://localhost:5000` in your web browser.

## Usage

### Upload a Movie

1. Click "Upload Movie" in the navigation
2. Enter the movie title
3. Select or drag-and-drop your video file
4. Optionally enter the duration
5. Click "Upload Movie"
6. Wait for upload to complete (shows progress)

### Watch a Movie

1. Click on any movie card on the home page or library
2. The video player will open
3. Use the built-in controls (play, pause, volume, fullscreen)

### Search Movies

2. Click the "Delete Video" button

## Project Structure

```
video-streaming-app/
├── public/
│   ├── index.html       # Main HTML file
│   ├── styles.css       # Responsive styling
│   └── uploads/         # Video storage
├── server.js            # Express server
├── package.json         # Dependencies
├── .env                 # Configuration
└── README.md            # This file
```

## API Endpoints

### Upload Video
- **POST** `/api/upload`
- Body: FormData with `video` file and optional `title`
- Returns: Video object with ID

### Get All Videos
- Returns: Array of video objects

### Get Video by ID
- Returns: Video file with streaming headers
### Delete Video
- **DELETE** `/api/videos/:id`
- Returns: Success message


Edit `.env` file to change:
## Mobile Optimization
The website is fully responsive and optimized for:
- **Mobile Phones** (320px - 480px): Optimized touch controls, stacked layout
- **Tablets** (481px - 768px): Adjusted grid and spacing
- **Desktops** (769px+): Full featured layout

## Performance Tips

1. **Video Encoding**: Use H.264 codec for best compatibility
   ```bash
   ```

2. **Large Files**: Split very large files before uploading

3. **Storage**: Monitor disk space for uploaded videos
4. **Browser Caching**: Clear browser cache if videos don't play

## Troubleshooting

### Videos won't upload
- Check file format is supported
- Verify file size is under 5GB
- Check disk space available
- Enable JavaScript in browser

### Videos won't play
- Ensure browser supports HTML5 video
- Try different video format (MP4 recommended)
- Check browser console for errors
- Clear browser cache

### Slow uploads
- Check internet connection
- Try smaller file sizes
- Close other applications using bandwidth

### 404 Not Found errors
- Make sure server is running on port 5000
- Restart the server
- Clear browser cache

## Security Considerations

For production use:

1. **Add Authentication**: Implement user login system
2. **Add Rate Limiting**: Prevent abuse with rate limits
3. **Validate Uploads**: Verify video files before storing
4. **Add Virus Scanning**: Scan uploaded files
5. **Use HTTPS**: Implement SSL/TLS certificates
6. **Add File Size Limits**: Adjust limits per your needs

## Future Enhancements

- [ ] User authentication system
- [ ] Comments and ratings
- [ ] Video thumbnails generation
- [ ] Automatic quality adjustment
- [ ] Video categories and tags
- [ ] Watch history
- [ ] Favorites/Bookmarks
- [ ] Playlist support
- [ ] Subtitle support
- [ ] Admin dashboard
- [ ] Analytics and statistics
- [ ] Social sharing

## License

MIT License - Feel free to use and modify

## Support

For issues or questions, check:
1. Browser console for error messages
2. Server logs for backend errors
3. Ensure videos are in supported format
4. Try refreshing the page

## Credits

Built with:
- Node.js & Express
- HTML5 Video
- CSS3 with Responsive Design
- Font Awesome Icons
- Vanilla JavaScript

---

**Enjoy your video streaming experience! 🎬🍿**
