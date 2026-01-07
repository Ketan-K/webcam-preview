# 📹 Webcam Preview Tool

> **A sleek, zero-install browser tool that turns your webcam into a professional preview station**

Ever needed to quickly check your webcam before a meeting? Want to test multiple cameras without installing bloatware? Need to zoom in on specific details? This lightweight, privacy-focused tool does it all—right in your browser.

**🌐 [Try it now - Live Demo](https://ketan-k.github.io/webcam-preview/)**

## ✨ What Makes This Special

🚀 **Instant Start** - Opens and auto-starts your camera in under a second  
🎥 **Multiple Cameras** - Seamlessly switch between all your connected webcams  
🔍 **Pro Zoom** - Select any area with your mouse to zoom up to 5x  
👻 **Ghost Mode** - Controls fade away when you're not moving the mouse  
📸 **One-Click Captures** - Screenshot with a single button press  
⚡ **Lightning Fast** - No installation, no loading, just pure performance  
🔒 **100% Private** - Everything runs locally—your video never leaves your browser

## 🎯 Perfect For

- 💼 Pre-meeting camera checks
- 🎬 Content creators testing setups
- 🔧 Webcam hardware testing
- 🎨 Frame composition and lighting tests
- 📷 Quick screenshot captures
- 🔬 Detailed inspection with zoom

## 🚀 Quick Start

### Option 1: Use Online (Fastest)
**👉 [Open Live Demo](https://ketan-k.github.io/webcam-preview/)** - Start using it right now!

### Option 2: Download & Run Locally
1. **Download** → Save `index.html` to your computer
2. **Open** → Double-click the file
3. **Allow** → Grant camera permission (one-time only)
4. **Done!** → Your camera starts automatically

That's it. No npm install. No pip install. No package managers. Just pure HTML5 magic.

## 🎮 How to Use

### The Basics

| What You Do | What Happens |
|------------|--------------|
| 🖱️ **Move Mouse** | Controls appear like magic |
| 🎯 **Click & Drag** | Select an area → Instant zoom |
| 👆 **Single Click** | Reset zoom back to normal |
| 🎥 **Click Camera** | Switch to that camera |
| 🖥️ **Fullscreen** | Immersive fullscreen mode |
| 📸 **Screenshot** | Download current frame |
| ⏹️ **Stop** | Turn off the camera |

### Pro Tips

💡 **Invisible Interface**: Controls auto-hide after 3 seconds—move your mouse to bring them back  
💡 **Precise Zoom**: The smaller your selection box, the bigger the zoom  
💡 **Quick Reset**: Just click once anywhere on the video  
💡 **Smooth Switching**: Camera switching is instant—no interruption

## 🎨 Features Deep Dive

### 🎬 Auto-Start Magic
The moment you open the tool, boom—your camera is live. No clicking through menus, no configuration screens. Just instant preview.

### 🔍 Zoom Like a Pro
Want to check if your hair is perfect? Or inspect that sticky note in the background?
1. Click and drag a box around any area
2. Release your mouse
3. BOOM—instant zoom up to 5x magnification
4. Click once anywhere to zoom back out

Minimum selection: 50×50 pixels (prevents accidental tiny zooms)

### 👻 Invisible UI
The interface knows when to get out of your way:
- **Move mouse** → Controls smoothly fade in
- **Stop moving** → After 3 seconds, everything fades out
- **Perfect for** → Clean screenshots and unobstructed viewing

### 🎥 Multi-Camera Maestro
Got multiple webcams? External camera? The tool finds them all:
- Hover to see your camera list
- Click any camera to switch instantly
- Active camera is highlighted
- Device names shown clearly

### 📊 Real-Time Stats
Hover the bottom-right to see:
- **Camera Name** → Which device is active
- **Resolution** → Exact pixel dimensions (e.g., 1920 × 1080)
- **Aspect Ratio** → For composition nerds (e.g., 1.78:1)

### 📸 Screenshot Superpowers
One click saves the current frame as a PNG:
- Full resolution capture
- Timestamped filename
- Downloads instantly
- Zero quality loss

## 💻 Browser Compatibility

| Browser | Minimum Version | Status |
|---------|----------------|--------|
| 🟢 Chrome | 88+ | Fully Supported |
| 🟢 Edge | 88+ | Fully Supported |
| 🛠️ Technical Stack

Built with the modern web platform:

- **WebRTC API** → Native camera access
- **Vanilla JavaScript (ES6+)** → Zero dependencies
- **CSS3** → Glassmorphism effects with backdrop filters
- **HTML5 Canvas** → Screenshot rendering
- **Media Streams API** → Multi-camera management

**File Size**: ~8KB (yes, kilobytes!)  
**Load Time**: < 100ms  
**Dependencies**: None. Nada. Zero.

## 📁 Project Structure

```
index.html              # The whole app
README.md         # This file
```

Yep, it's literally one file. That's the point.

## 🚀 For Developers

### Want to Customize?

Just open `index.html` in your favorite editor:

```html
<!-- Change zoom limits -->
const scale = Math.min(scaleX, scaleY, 5); // Change 5 to whatever

<!-- Adjust auto-hide timer -->
mouseTimer = setTimeout(() => {...}, 3000); // Change 3000 (3 sec)

<!-- Modify resolution request -->
width: { ideal: 1920 },  // Request different resolution
height: { ideal: 1080 }
```

### No Build Process Needed

- Edit the HTML file
- Refresh your browser
- That's it

### Tech Highlights

```javascript
// Clean async/await camera enumeration
const devices = await navigator.mediaDevices.enumerateDevices();

// Smooth transform animations
transform: scale(${scale}) translate(${offsetX}%, ${offsetY}%);

// Instant screenshot with canvas
ctx.drawImage(elements.video, 0, 0);
canvas.toBlob(blob => download(blob));
```

## 🎯 Use Cases

### 👔 Corporate
- Pre-meeting camera checks
- Test new webcam installations
- Verify video quality before calls

### 🎥 Content Creation
- Frame your shot perfectly
- Check lighting and composition
- Test multiple camera angles

### 🔧 Troubleshooting
- Verify webcam is working
- Compare multiple cameras
- Check actual resolution

### 🎨 Creative
- Zoom for detail work
- Capture reference photos
- Test camera positions

## 🤔 FAQ

**Q: Does this work offline?**  
A: Yes! After the first load, it works without internet.

**Q: Can I use this on mobile?**  
A: Yes! Works on mobile browsers with camera support.

**Q: Where are screenshots saved?**  
A: Your browser's default download folder with timestamp.

**Q: Is my video recorded?**  
A: Nope. Nothing is recorded unless you click screenshot.

**Q: Why is it so fast?**  
A: No frameworks, no bundlers, no bloat—just pure browser APIs.

**Q: Can I embed this in another page?**  
A: Absolutely! Just iframe it or copy the code.

## 🌟 Why This Exists

Because in 2026, you shouldn't need to:
- Install a 500MB app to test your webcam
- Sign up for an account to preview your camera
- Upload your video to a server to take a screenshot
- Navigate through 10 menus to switch cameras

This tool does one thing, does it well, and respects your privacy.

## 📄 License

Free to use, modify, and distribute. No strings attached.

## 🤝 Contributing

Found a bug? Want a feature? The HTML is right there—fork it, fix it, share it!

---

<div align="center">

**Made with 💜 for anyone who just wants to check their webcam without the hassle**

*No tracking • No servers • No nonsense*

⭐ Star this repo if it saved you from installing yet another app

</div>

