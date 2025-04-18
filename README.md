# video-downloader

A web application that allows users to download videos from various platforms like YouTube, Facebook, Instagram, and more.

## Features
- Support for multiple video platforms (YouTube, Facebook, Instagram, TikTok)
- Multiple quality options
- Fast and efficient downloads
- Modern and responsive UI
- Cross-platform compatibility

## Tech Stack
- Frontend: React + TypeScript + Vite
- Backend: Python + FastAPI
- Video Download: yt-dlp

## Deployment Instructions

### Backend Deployment (Render.com)

1. Create a new account on [Render.com](https://render.com)
2. Create a new Web Service
3. Connect your GitHub repository
4. Configure the service:
   - Name: video-downloader-backend
   - Environment: Python
   - Build Command: `pip install -r requirements.txt`
   - Start Command: `uvicorn src.pages.api.ytdlp_new:app --host 0.0.0.0 --port $PORT`
   - Python Version: 3.11.0
5. Deploy the service
6. Copy the provided URL (e.g., https://your-backend-url.onrender.com)

### Frontend Deployment (Netlify)

1. Create a new account on [Netlify](https://netlify.com)
2. Create a new site from Git
3. Connect your GitHub repository
4. Configure the build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
5. Add environment variable:
   - Key: `VITE_API_URL`
   - Value: Your backend URL from Render.com
6. Deploy the site

## Local Development

### Backend

1. Install Python 3.11
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Start the server:
   ```bash
   cd src/pages/api
   uvicorn ytdlp_new:app --reload --host 0.0.0.0 --port 8000
   ```

### Frontend

1. Install Node.js
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## Environment Variables

### Backend
- `PYTHON_VERSION`: Python version to use (default: 3.11.0)

### Frontend
- `VITE_API_URL`: Backend API URL (default: http://localhost:8000)

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
#   v i d e o - d o w n l o a d e r  
 #   Y T - M P -  
 