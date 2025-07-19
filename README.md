# Colorful Dino Run Game - Hostinger Deployment Guide

## About
This is a standalone HTML5 game that recreates the classic dinosaur running game with colorful obstacles. The game works on both desktop and mobile devices without requiring any server setup.

## Files Included
- `index.html` - Complete game file (contains HTML, CSS, and JavaScript)

## Features
- ✅ Works on desktop and mobile devices
- ✅ Touch controls for mobile devices
- ✅ Keyboard controls for desktop (SPACEBAR to jump)
- ✅ Progressive difficulty - gets faster as score increases
- ✅ Colorful obstacles with random colors
- ✅ High score tracking (saved in browser)
- ✅ Responsive design that adapts to screen size
- ✅ Beautiful graphics with sky gradient and moving clouds

## How to Deploy on Hostinger

### Step 1: Access Your Hostinger Control Panel
1. Log in to your Hostinger account at https://www.hostinger.com
2. Go to your hosting control panel (hPanel)
3. Find your domain/website and click "Manage"

### Step 2: Upload the Game Files
1. In hPanel, click on "File Manager"
2. Navigate to the "public_html" folder (this is where your website files go)
3. If you want the game as your main website:
   - Upload `index.html` directly to the `public_html` folder
   - Your game will be available at `yourdomain.com`

4. If you want the game in a subfolder (recommended):
   - Create a new folder inside `public_html` (e.g., "game" or "dino-run")
   - Upload `index.html` to this new folder
   - Your game will be available at `yourdomain.com/game/` or `yourdomain.com/dino-run/`

### Step 3: Set File Permissions (if needed)
1. Right-click on the uploaded `index.html` file
2. Select "Permissions" or "Change Permissions"
3. Set permissions to 644 (read/write for owner, read for group and others)

### Step 4: Test Your Game
1. Open your web browser
2. Go to your domain: `yourdomain.com` or `yourdomain.com/your-folder-name/`
3. The game should load immediately
4. Test on both desktop (use SPACEBAR) and mobile (tap to jump)

## Alternative Upload Methods

### Using FTP Client (FileZilla, etc.)
1. Download an FTP client like FileZilla
2. Connect using your Hostinger FTP credentials:
   - Host: your domain or FTP server
   - Username: your FTP username
   - Password: your FTP password
   - Port: 21 (or 22 for SFTP)
3. Navigate to the `public_html` folder
4. Upload the `index.html` file

### Using Hostinger Website Builder
1. If you're using Hostinger's website builder, you can embed the game:
2. Create a new page or section
3. Add an HTML widget
4. Copy and paste the entire content of `index.html` into the HTML widget

## Troubleshooting

### Game doesn't load
- Check that the file is named exactly `index.html` (lowercase)
- Verify the file is in the correct directory (`public_html` or subdirectory)
- Check file permissions are set to 644

### Game loads but doesn't work on mobile
- Ensure you're testing on a mobile device or mobile browser mode
- The game auto-detects mobile devices and enables touch controls

### High scores don't save
- This is normal behavior - high scores are saved locally in each browser
- Each visitor will have their own high score tracking

## Technical Details
- **File Size**: Single HTML file (~15KB)
- **Browser Support**: Works in all modern browsers (Chrome, Firefox, Safari, Edge)
- **Mobile Support**: Full touch support for iOS and Android
- **Dependencies**: None - completely self-contained
- **Server Requirements**: None - works on any web hosting that supports HTML files

## Customization
You can easily customize the game by editing the `index.html` file:
- Change colors in the `config.colors` array
- Adjust game speed by modifying `config.gameSpeed`
- Change jump power with `config.jumpPower`
- Modify obstacle generation rates

## Support
If you encounter any issues during deployment, check:
1. File permissions are correct (644)
2. File is in the right directory (`public_html`)
3. File name is exactly `index.html`
4. Your domain is properly pointed to your hosting account

Enjoy your colorful dinosaur game!