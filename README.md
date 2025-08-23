# 🔦 Mobile Flashlight Web App

A simple, responsive web-based flashlight app that uses your mobile device's camera flash. Perfect for quick access to a flashlight directly from your browser!

## ✨ Features

- 🎯 **One-click flashlight activation**
- 📱 **Mobile-optimized responsive design**
- 🌙 **Dark theme with glowing animations**
- ⚡ **Uses device camera flash/torch**
- 🔒 **No data collection or tracking**
- 🚀 **Works offline after first load**

## 🚀 Live Demo

**Access the app here:** [https://yourusername.github.io/flashlight-app](https://inajmudinov.github.io/flashlight-app)

*Replace `yourusername` with your actual GitHub username*

## 📱 Browser Compatibility

| Browser | Android | iOS | Support Level |
|---------|---------|-----|---------------|
| Chrome | ✅ Excellent | ✅ Excellent | Full flashlight control |
| Safari | ⚠️ Limited | ✅ Excellent | Works on most devices |
| Firefox | ❌ Poor | ❌ Poor | Limited API support |
| Edge | ⚠️ Limited | ⚠️ Limited | Varies by device |

## 🛠️ Setup Instructions

### Quick Deploy to GitHub Pages

1. **Fork or clone this repository**
   ```bash
   git clone https://github.com/yourusername/flashlight-app.git
   ```

2. **Enable GitHub Pages**
   - Go to your repository settings
   - Scroll to "Pages" section  
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

3. **Access your app**
   - Your app will be available at: `https://yourusername.github.io/flashlight-app`
   - It may take a few minutes to deploy

### Local Development

```bash
# Clone the repository
git clone https://github.com/yourusername/flashlight-app.git

# Navigate to directory
cd flashlight-app

# Serve locally (requires HTTPS for camera access)
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server -p 8000
```

**Note:** For camera access, you'll need to serve over HTTPS in production.

## 🔧 How It Works

The app uses the modern **MediaDevices API** to access your device's camera and control the torch/flash:

1. **Camera Access**: Requests permission to use the rear camera
2. **Torch Control**: Applies torch constraints to enable/disable flash
3. **Responsive Design**: Adapts to different screen sizes
4. **Error Handling**: Gracefully handles unsupported devices/browsers

## ⚠️ Troubleshooting

### "Permission denied" Error

**Quick Fixes:**
- ✅ Use Chrome or Safari browser
- ✅ Ensure you're on HTTPS (GitHub Pages provides this)
- ✅ Allow camera permissions when prompted
- ✅ Refresh page and try again

**Browser Settings:**
- **Chrome**: Settings → Site settings → Camera → Allow
- **Safari**: Settings → Safari → Camera → Allow for this site

### App Not Working?

**Check these requirements:**
- 📱 Mobile device with camera flash
- 🌐 Modern browser (Chrome/Safari recommended) 
- 🔒 HTTPS connection (required for camera API)
- 📷 Camera permissions granted

### Common Issues

| Issue | Solution |
|-------|----------|
| No flash detected | Device may not have controllable flash |
| Permissions blocked | Check browser settings, refresh and retry |
| App won't load | Ensure GitHub Pages is enabled |
| Button not responding | Try different browser (Chrome recommended) |

## 🔐 Privacy & Security

- **No data collection**: App runs entirely in your browser
- **No external requests**: All code is self-contained
- **Camera access**: Only used for flash control, no recording
- **Open source**: Full code available for review

## 🛠️ Technical Details

- **Pure HTML/CSS/JavaScript**: No frameworks or dependencies
- **Camera API**: Uses `navigator.mediaDevices.getUserMedia()`
- **Torch Control**: Applies `torch: true` constraint to video track
- **Responsive**: CSS Grid and Flexbox for mobile optimization
- **Progressive Enhancement**: Graceful fallback for unsupported devices

## 📂 File Structure

```
flashlight-app/
├── index.html          # Main app file (complete single-file app)
├── README.md          # This file
└── LICENSE            # MIT License (optional)
```

## 🤝 Contributing

Contributions are welcome! Here are ways to contribute:

1. **Report Issues**: Found a bug? Open an issue
2. **Suggest Features**: Have ideas? Create a feature request  
3. **Submit PRs**: Improve the code and submit a pull request
4. **Test Devices**: Try on different devices and report compatibility

### Development Guidelines

- Keep it simple (single HTML file)
- Maintain mobile-first design
- Ensure cross-browser compatibility
- Add proper error handling

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Built with vanilla JavaScript for maximum compatibility
- Inspired by the need for a simple, web-based flashlight
- Thanks to the web community for Camera API documentation

---

**⭐ Star this repo if it helped you!**

**🐛 Found an issue?** [Report it here](https://github.com/yourusername/flashlight-app/issues)

**💡 Have suggestions?** [Start a discussion](https://github.com/yourusername/flashlight-app/discussions)

---

*Made with ❤️ for mobile users who need a quick flashlight solution*
