# 🚀 XR_EdSpace Deployment Guide

Complete step-by-step guide to deploy your XR_EdSpace AR platform to GitHub Pages.

---

## ⚠️ CRITICAL: Compile Markers FIRST!

**YOU MUST DO THIS BEFORE UPLOADING TO GITHUB!**

The `assets/targets.mind` file is currently a PLACEHOLDER. Without compiling the markers, the AR experience will show infinite loading screen.

---

## 📋 Pre-Deployment Checklist

- [ ] Extract the XR_EdSpace package
- [ ] Compile AR markers (see below)
- [ ] Replace `assets/targets.mind` with compiled file
- [ ] Verify all files are present
- [ ] Have GitHub account ready

---

## Step 1: Compile AR Markers (REQUIRED)

### Method: Online Compiler (Easiest)

1. **Open the compiler:**
   - Go to: https://hiukim.github.io/mind-ar-js-doc/tools/compile/

2. **Upload FIRST marker:**
   - Click "Drop files here to upload"
   - Select `markers/heart_anatomy_marker.jpg`
   - You should see a thumbnail appear

3. **Upload SECOND marker:**
   - Click the upload area again
   - Select `markers/brain_anatomy_marker.jpg`
   - You should now see TWO thumbnails

4. **Start compilation:**
   - Click the green "Start" button
   - Wait 30-60 seconds (progress will show)
   - **Do NOT close the page!**

5. **Download compiled file:**
   - When complete, `targets.mind` will download automatically
   - Save it to your computer

6. **Replace placeholder:**
   - Delete `assets/targets.mind` from the package
   - Move the downloaded `targets.mind` into `assets/` folder

**IMPORTANT:** 
- Upload markers in the EXACT order (heart first, brain second)
- If compilation fails, refresh and try again
- The compiled file should be 50KB-500KB (not 53 bytes!)

---

## Step 2: Deploy to GitHub Pages

### Option A: Web Interface (No Command Line)

#### 2.1 Create Repository

1. **Go to GitHub:**
   - Visit: https://github.com/new
   - Log in if needed

2. **Configure repository:**
   - **Repository name:** `XR-EdSpace-MVP` (or your choice)
   - **Description:** "AR-powered Living Textbook platform"
   - **Visibility:** Public (required for free GitHub Pages)
   - **Do NOT check** "Add README" or any initialization options
   - Click "Create repository"

#### 2.2 Upload Files

1. **On the new repository page:**
   - Click "uploading an existing file" link

2. **Upload all files:**
   - **Method 1 (Drag & Drop):**
     - Open the XR_EdSpace folder on your computer
     - Select ALL files and folders
     - Drag them into the GitHub upload area
   
   - **Method 2 (Browse):**
     - Click "choose your files"
     - Select all files (Ctrl+A or Cmd+A)
     - Click Open

3. **Commit files:**
   - Scroll down
   - Add commit message: "Initial deployment of XR_EdSpace v1.2"
   - Click "Commit changes"

#### 2.3 Enable GitHub Pages

1. **Go to Settings:**
   - Click "Settings" tab at top of repository

2. **Navigate to Pages:**
   - Click "Pages" in left sidebar

3. **Configure source:**
   - Under "Source", select "main" branch
   - Leave folder as "/ (root)"
   - Click "Save"

4. **Wait for deployment:**
   - GitHub will show "Your site is ready to be published"
   - Wait 2-3 minutes
   - Refresh the page
   - You'll see: "Your site is live at https://[username].github.io/[repo-name]/"

#### 2.4 Test Your Deployment

1. **Open the URL:**
   - Click the provided GitHub Pages URL
   - Add `/demo.html` to the end
   - Example: `https://fahim749.github.io/XR-EdSpace-MVP/demo.html`

2. **Verify demo page:**
   - Should see the landing page with markers
   - Check that images load correctly
   - Click "Launch AR Experience"

3. **Test AR on mobile:**
   - Open the same URL on your smartphone
   - Grant camera permissions
   - Camera should load (not infinite loading!)
   - Point at printed marker
   - 3D model should appear

---

## Step 3: Verify Everything Works

### Desktop Verification

- [ ] Demo page loads correctly
- [ ] Both marker images are visible
- [ ] Credits section appears at bottom
- [ ] "Launch AR Experience" button works
- [ ] AR page shows camera permission request

### Mobile Verification

- [ ] Demo page loads on mobile
- [ ] AR page requests camera access
- [ ] Camera view appears (not stuck loading!)
- [ ] Heart marker triggers heart model
- [ ] Brain marker triggers brain model
- [ ] Can rotate model by dragging
- [ ] Can zoom with pinch gesture
- [ ] Can pan with two fingers
- [ ] Long press pauses/resumes rotation
- [ ] Info panel shows model facts

---

## 🔧 Troubleshooting

### Issue: Infinite Loading Screen

**Cause:** Placeholder `targets.mind` file not replaced

**Solution:**
1. Download compiled `targets.mind` from MindAR compiler
2. In GitHub, navigate to `assets/targets.mind`
3. Click the file, then click trash icon to delete
4. Go back to `assets/` folder
5. Click "Add file" → "Upload files"
6. Upload the compiled `targets.mind`
7. Commit changes
8. Wait 2-3 minutes and test again

### Issue: Camera Permission Denied

**Cause:** Browser security or HTTPS issue

**Solution:**
- Ensure you're using HTTPS (GitHub Pages uses HTTPS automatically)
- Check browser settings for camera permissions
- Try a different browser (Chrome recommended)
- On iOS, use Safari; on Android, use Chrome

### Issue: Models Not Appearing

**Cause:** Marker not detected or poor lighting

**Solution:**
- Print marker on white paper (not screen display)
- Ensure good lighting
- Keep marker flat and fully visible
- Hold phone 20-40cm from marker
- Try different marker (heart or brain)

### Issue: Models Too Large/Small

**Cause:** Incorrect scaling in code

**Solution:**
- Heart should be 0.5x scale
- Brain should be 0.003x scale
- Check `index.html` for correct scale values

### Issue: Gestures Not Working

**Cause:** JavaScript error or touch events not registered

**Solution:**
- Check browser console for errors
- Ensure you're testing on actual mobile device (not desktop)
- Try refreshing the page
- Clear browser cache

---

## 📊 Deployment Checklist

### Pre-Upload
- [ ] Markers compiled successfully
- [ ] `targets.mind` file replaced (not placeholder)
- [ ] All files present in package
- [ ] Models in `models/` folder
- [ ] Markers in `markers/` folder

### GitHub Setup
- [ ] Repository created
- [ ] All files uploaded
- [ ] GitHub Pages enabled
- [ ] Deployment successful

### Testing
- [ ] Demo page loads
- [ ] AR page loads
- [ ] Camera initializes
- [ ] Heart marker works
- [ ] Brain marker works
- [ ] All gestures work
- [ ] Attribution visible

---

## 🎯 Next Steps After Deployment

1. **Print Markers:**
   - Print both markers on white paper
   - A4 or Letter size recommended
   - High quality print for best tracking

2. **Test Thoroughly:**
   - Test on multiple devices
   - Try different lighting conditions
   - Verify all features work

3. **Share:**
   - Share the demo URL with your adviser
   - Prepare your pitch presentation
   - Gather feedback from users

4. **Iterate:**
   - Document user feedback
   - Plan improvements
   - Consider additional models

---

## 💡 Pro Tips

### For Best AR Experience
- **Lighting:** Bright, even lighting works best
- **Distance:** Hold phone 20-40cm from marker
- **Angle:** Keep marker flat, camera perpendicular
- **Stability:** Keep marker and phone steady

### For Demos
- **Print Quality:** Use high-quality printer
- **Paper:** White, non-glossy paper
- **Size:** Full A4/Letter size (don't scale down)
- **Backup:** Have digital copy on second device

### For Development
- **Local Testing:** Use `python3 -m http.server 8080`
- **HTTPS:** Required for camera access
- **Console:** Check browser console for errors
- **Cache:** Clear cache when testing updates

---

## 📞 Need Help?

If you encounter issues:

1. **Check this guide** - Most issues are covered here
2. **Verify markers compiled** - This is the #1 issue
3. **Check browser console** - Look for error messages
4. **Test on different device** - Rule out device-specific issues
5. **Review GitHub Actions** - Check deployment logs

---

## ✅ Success Criteria

Your deployment is successful when:

✅ Demo page loads without errors
✅ AR page initializes camera
✅ Both markers trigger 3D models
✅ All gestures work smoothly
✅ Models are properly scaled
✅ Attribution section visible
✅ No console errors

---

**You're ready to transform education with AR!** 🚀

*For additional support, see README.md or contact the XR_EdSpace team.*
