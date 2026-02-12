# 📸 ChronoFrame - Offline Photo Timeline Organizer

> A 100% offline, privacy-first photo timeline application that organizes your photos by date using EXIF metadata. No upload, no cloud, just your photos on your computer.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![Offline](https://img.shields.io/badge/offline-100%25-orange.svg)

## ✨ Features

- 📁 **Folder Scanning** - Select entire folders, not individual files
- 📅 **Smart Timeline** - Auto-organizes by Year → Month from EXIF data
- 💾 **Smart Caching** - IndexedDB thumbnails for instant re-loading
- 📐 **Customizable Grid** - Choose 2×2, 3×3, 4×4, 5×5, or Auto layout
- 🎯 **Timeline Navigator** - Draggable date picker to jump anywhere
- 🔒 **100% Offline** - Everything happens locally, zero uploads
- 📱 **Responsive Design** - Works on desktop, tablet, and mobile
- 🖼️ **Format Support** - JPG, PNG, HEIC (iPhone), WEBP, GIF, BMP, TIFF

## 🚀 Quick Start

### Option 1: Direct Use
1. Download `photo-timeline.html`
2. Double-click to open in your browser
3. Click "Scan a Folder" and select your photos folder
4. Done! Photos organized by timeline

### Option 2: Clone Repository
```bash
git clone https://github.com/yourusername/chronoframe.git
cd chronoframe
# Open photo-timeline.html in your browser
```

## 🎮 How to Use

### 1. Scan Photos
- Click **"Scan a Folder"** → Select any folder with photos
- Or click **"Select Individual Photos"** → Choose specific files
- App reads EXIF metadata and organizes by date

### 2. Browse Timeline
- Photos organized by **Year → Month**
- Click **📅 button** (bottom-right) for timeline navigator
- **Drag navigator** to move it anywhere
- Click any **year/month** to jump instantly

### 3. Customize View
- Switch between **Timeline** and **Grid** views
- Choose grid size: **2×2, 3×3, 4×4, 5×5, or Auto**
- Grid applies to both views

### 4. View Photos
- Click any photo → Full-screen modal with metadata
- Shows: Date, Time, Camera, Resolution, Settings
- Press **ESC** or click **X** to close

## 🔒 Privacy & Security

### What Stays Local
✅ All photos remain on your hard disk  
✅ Thumbnails cached in browser IndexedDB  
✅ No internet connection required  
✅ No servers, no cloud, no upload  
✅ Zero tracking or analytics  

### Before Sharing This App on GitHub

**⚠️ IMPORTANT:** Click **💣 Clear Cache (GitHub)** button before pushing to Git!

This will:
- Delete all cached thumbnails from IndexedDB
- Clear all photo data from memory
- Remove any trace of your personal photos

The app itself contains **zero photo data** - it's just code. But cached thumbnails in your browser need to be cleared manually.

## 🛠️ Technical Details

### Single File Architecture
- **No build process** - Pure HTML/CSS/JS
- **No dependencies** - Everything in one file (except CDN libraries)
- **No installation** - Just open and use

### Technologies
- React 18 (UI framework)
- EXIF.js (metadata extraction)
- IndexedDB (local caching)
- Canvas API (thumbnail generation)
- CSS Grid (responsive layouts)

### Browser Support
- ✅ Chrome 90+ (Recommended)
- ✅ Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+

### Format Support
| Format | Support | Notes |
|--------|---------|-------|
| JPG/JPEG | ✅ Full | Most common format |
| PNG | ✅ Full | Transparent backgrounds |
| HEIC/HEIF | ✅ Full | iPhone photos (iOS 11+) |
| WEBP | ✅ Full | Modern format |
| GIF | ✅ Full | Animated supported |
| BMP | ✅ Full | Legacy format |
| TIFF | ✅ Full | Professional format |

## 📖 Features Explained

### 💾 Smart Caching
First scan: Processes all photos, creates thumbnails  
Second scan: **Instant loading from cache!** ⚡  
- Thumbnails stored in browser IndexedDB
- Automatically cleaned after 30 days
- Shows cache stats in header

### 📅 Timeline Navigator
- Floating panel showing all years/months
- **Draggable** - position it anywhere
- Click to jump instantly to any date
- Shows photo count per month
- Active selection highlighted in gold

### 🔗 Share Feature
Export privacy-safe HTML file with:
- ❌ NO GPS location
- ❌ NO camera info  
- ❌ NO file names
- ✅ Just photos and dates

Perfect for sharing vacation photos without metadata!

## 🎯 Use Cases

- 📸 **Personal Photo Organization** - Organize thousands of photos effortlessly
- 🏖️ **Vacation Memories** - Browse trips by date
- 📱 **iPhone Photo Management** - Full HEIC support
- 👨‍👩‍👧 **Family Archives** - Organize family photos by timeline
- 🎂 **Event Photos** - Weddings, birthdays, parties
- 🔒 **Privacy-Conscious Users** - No cloud required

## 🐛 Troubleshooting

### Photos Not Loading
- **Check format**: Only image files supported
- **Check EXIF**: Photos without EXIF use file modification date
- **Check browser**: Use Chrome/Edge for best compatibility

### Folder Selection Not Working
- **Browser support**: Chrome/Edge have best folder selection support
- **Try Firefox**: Also fully supported
- **Safari**: Works on Safari 14+

### HEIC Files Not Displaying
- **Best support**: Chrome, Edge, Safari
- **Limited support**: Firefox may have issues
- **Alternative**: Convert HEIC to JPG on iPhone (Settings → Camera → Formats → Most Compatible)

### Cache Not Working
- **Private mode**: IndexedDB disabled in incognito
- **Browser storage**: Check if storage enabled
- **Clear and retry**: Use "Clear Cache (GitHub)" button

## 🤝 Contributing

Contributions welcome! Here's how:

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. **Clear cache** before committing (`💣 Clear Cache (GitHub)` button)
4. Commit changes (`git commit -m 'Add AmazingFeature'`)
5. Push to branch (`git push origin feature/AmazingFeature`)
6. Open Pull Request

### Before Submitting PR
- [ ] Click **💣 Clear Cache (GitHub)** button
- [ ] Test in Chrome, Firefox, Edge
- [ ] Verify no personal photos in cache
- [ ] Update README if adding features

## 📝 License

MIT License - feel free to use, modify, and distribute!

## 🙏 Credits

- **EXIF.js** - Jacob Seidelin (EXIF metadata extraction)
- **React** - Facebook (UI framework)
- **Fonts** - Google Fonts (Playfair Display, DM Sans)

## 📧 Support

- 🐛 **Bug Reports**: Open an issue on GitHub
- 💡 **Feature Requests**: Open an issue with [FEATURE] tag
- 📖 **Documentation**: Check `README.md` and `QUICK_START.md`

## 🎉 What Makes ChronoFrame Special?

1. **Truly Offline** - Not "offline-first", but **offline-only**
2. **Privacy First** - Your photos never leave your computer
3. **No Setup** - Just open and use
4. **Smart Caching** - Fast re-loading without reprocessing
5. **Beautiful UI** - Vintage photography aesthetic
6. **Open Source** - Free forever, modify as you like

---

**Built with ❤️ for photography enthusiasts who value privacy**

⭐ If you find this useful, please star the repository!
