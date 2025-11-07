# XR_EdSpace - Living Textbook AR Platform

Transform traditional textbooks into interactive augmented reality experiences. Scan printed diagrams with your smartphone to explore 3D anatomical models.

## 🎯 Features

- ✅ **Multi-Image AR Tracking** - Heart and brain anatomy models
- ✅ **Interactive 3D Models** - High-quality anatomical models
- ✅ **Full Gesture Controls** - Rotate, zoom, pan with intuitive touch gestures
- ✅ **Long-Press to Pause** - Control automatic rotation
- ✅ **Web-Based** - No app installation required
- ✅ **Mobile Optimized** - Works on iOS and Android devices
- ✅ **Professional UI** - Clean, educational interface
- ✅ **Complete Attribution** - All assets properly credited

## 📱 Quick Start

### For Users

1. Visit the demo page on your mobile device
2. Print one of the AR markers (heart or brain)
3. Click "Launch AR Experience"
4. Point your camera at the printed marker
5. Interact with the 3D model using touch gestures

### For Developers

**IMPORTANT: You MUST compile the AR markers before deployment!**

## 🔧 Deployment Instructions

### Step 1: Compile AR Markers

**This step is REQUIRED before deployment!**

1. Go to: https://hiukim.github.io/mind-ar-js-doc/tools/compile/
2. Upload markers **in this exact order**:
   - FIRST: `markers/heart_anatomy_marker.jpg`
   - SECOND: `markers/brain_anatomy_marker.jpg`
3. Click "Start" and wait for compilation (30-60 seconds)
4. Download the `targets.mind` file
5. Replace `assets/targets.mind` with the downloaded file

### Step 2: Deploy to GitHub Pages

1. Create a new GitHub repository
2. Upload all files from this folder
3. Go to Settings → Pages
4. Select "main" branch as source
5. Save and wait 2-3 minutes
6. Access at: `https://[username].github.io/[repo-name]/demo.html`

## 🎮 Interactive Controls

| Gesture | Action | Description |
|---------|--------|-------------|
| 👆 **Drag** | Rotate | Drag with one finger to rotate model |
| 🤏 **Pinch** | Zoom | Pinch with two fingers to zoom (0.3x - 8x) |
| ✌️ **Two Fingers** | Pan | Drag with two fingers to reposition |
| ⏸️ **Long Press** | Pause/Resume | Hold for 0.5s to pause/resume rotation |

## 📁 Project Structure

```
XR_EdSpace_FINAL_VERIFIED/
├── index.html              # Main AR application
├── demo.html               # Landing page with markers
├── README.md               # This file
├── LICENSE                 # MIT License
├── models/
│   ├── Heart__photor.glb   # Heart 3D model (2.2MB)
│   └── Brain_NIH3D.glb     # Brain 3D model (5.2MB)
├── markers/
│   ├── heart_anatomy_marker.jpg  # Heart AR marker
│   └── brain_anatomy_marker.jpg  # Brain AR marker
├── assets/
│   └── targets.mind        # Compiled AR tracking data (MUST REPLACE!)
└── docs/
    └── DEPLOYMENT_GUIDE.md # Detailed deployment instructions
```

## 🔬 Technical Specifications

- **AR Library:** MindAR v1.2.2 (MIT License)
- **3D Engine:** A-Frame v1.4.2 + Three.js (MIT License)
- **Compatibility:** iOS 11+, Android 7.0+, modern browsers
- **Requirements:** HTTPS, camera access, WebGL support
- **File Size:** ~7.5MB total (models + assets)
- **Performance:** 30+ FPS on mid-range smartphones

## 📊 Model Information

### Heart Model
- **File:** Heart__photor.glb (2.2MB)
- **Scale:** 0.5x (optimized for AR)
- **License:** CC Attribution
- **Features:** Photorealistic, detailed anatomy

### Brain Model
- **File:** Brain_NIH3D.glb (5.2MB)
- **Scale:** 0.003x (millimeter units converted)
- **License:** Public Domain (NIH)
- **Features:** High-resolution, anatomically accurate

## 🎓 Educational Use

Perfect for:
- Medical and nursing students
- Anatomy courses
- Biology education
- Interactive textbooks
- Museum exhibits
- Science demonstrations

## 📜 License & Attribution

### Platform
- **XR_EdSpace** © 2025
- **License:** MIT License
- Free for educational and commercial use

### 3D Models
- **Brain:** NIH 3D Print Exchange (Public Domain)
- **Heart:** Educational Model (CC Attribution)

### AR Markers
- **Base Images:** Vintage Medical Illustrations (Public Domain)
- **Sources:** The Graphics Fairy, Rawpixel

### Technology
- **MindAR:** MIT License - HiuKim Yuen
- **A-Frame:** MIT License
- **Three.js:** MIT License

See `demo.html` for complete attribution details.

## 🚀 Roadmap

- [ ] Add more anatomical models (lungs, liver, kidneys)
- [ ] Multi-language support
- [ ] Voice narration
- [ ] Quiz mode
- [ ] Model annotations
- [ ] Export to VR headsets

## 🤝 Contributing

We welcome contributions! This is an educational platform designed to make learning more interactive and accessible.

## 📞 Support

For questions, partnerships, or support:
- **Email:** contact@xredspace.com
- **Website:** https://xredspace.com
- **GitHub:** [Your GitHub URL]

## ⚠️ Important Notes

1. **MUST compile markers** before deployment (see Step 1 above)
2. **HTTPS required** for camera access
3. **Print markers on white paper** for best tracking
4. **Good lighting** improves AR performance
5. **Keep marker flat** and fully visible

## 🎉 Version History

### v1.2 (Current)
- ✅ Long-press to pause rotation
- ✅ Complete attribution system
- ✅ Improved gesture controls
- ✅ Better model scaling

### v1.1
- ✅ Multi-image tracking (heart + brain)
- ✅ Full gesture controls
- ✅ Professional UI/UX

### v1.0
- ✅ Initial release
- ✅ Single model AR tracking

---

**Built with ❤️ for students and educators worldwide**

*Transform textbooks. Transform learning. Transform education.*
