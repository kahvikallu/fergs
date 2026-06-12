# 🐸 Find the Frog Game

A fun "Find the Frog" game where you search for hidden frogs among lily pads! When you find all the frogs, you'll see a SoundCloud-style barcode on the final screen.

## How to Play

1. Click on the lily pads (🍃) to reveal what's underneath
2. Find all 5 frogs (🐸) hidden in the grid
3. Track your attempts and time
4. When you find all frogs, you'll see the victory screen with a SoundCloud barcode!

## Features

- 🎮 Interactive 26x10 grid gameplay
- ⏱️ Timer to track your speed
- 📊 Statistics tracking (attempts, time, frogs found)
- 🎨 Beautiful gradient design with animations
- 📱 Responsive design for mobile and desktop
- 🎉 Victory screen with SoundCloud-style barcode visualization
- 🔄 Play again functionality

## Hosting on GitHub Pages

To host this game on GitHub Pages:

### Option 1: Using GitHub UI

1. Create a new repository on GitHub (or use an existing one)
2. Upload the `index.html` file to the repository
3. Go to **Settings** → **Pages**
4. Under "Source", select your branch (usually `main` or `master`)
5. Click **Save**
6. Your game will be live at `https://yourusername.github.io/repository-name/`

### Option 2: Using Git Command Line

```bash
# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit changes
git commit -m "Add Find the Frog game"

# Add your remote repository (replace with your repo URL)
git remote add origin https://github.com/yourusername/your-repo-name.git

# Push to main branch
git push -u origin main
```

Then enable GitHub Pages in your repository settings as described above.

### Customizing the SoundCloud Barcode

To add your actual SoundCloud track:

1. Go to your SoundCloud track
2. Click **Share** → **Embed**
3. Copy the barcode/QR code image URL or create a custom barcode
4. Replace the SVG in the `.barcode-placeholder` section with your actual SoundCloud barcode image:

```html
<div class="soundcloud-barcode">
    <img src="YOUR_SOUNDCLOUD_BARCODE_URL.png" alt="SoundCloud Track">
</div>
```

Or link to your SoundCloud profile:

```html
<div class="barcode-placeholder" onclick="window.open('https://soundcloud.com/yourprofile', '_blank')" style="cursor: pointer;">
    <!-- barcode content -->
</div>
```

## Game Configuration

You can customize the game by editing these values in the JavaScript section:

- `GRID_SIZE`: Number of cells in the grid (default: 20 for 5x4)
- `TOTAL_FROGS`: Number of frogs to find (default: 5)

## License

Free to use and modify!

---

Made with 🐸 and 💚
