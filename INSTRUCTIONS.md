# Website Editing Guide

## Where to Edit Content

- **`content/home/`** - Homepage sections
- **`content/about/`** - About page
- **`content/authors/garbe/`** - Your profile
- **`content/publication/`** - Publications
- **`content/project/`** - Research projects
- **`content/talk/`** - Talks and presentations
- **`config/_default/config.toml`** - Site settings
- **`config/_default/params.toml`** - Theme and appearance

---

## How to Publish Changes to the Website

### Step 1: Build the Site

**Why use PowerShell?** GitHub Desktop cannot run Hugo directly - it's only for Git operations. You need PowerShell (or Command Prompt) to run the Hugo command that builds your website.

1. Open **PowerShell**

2. **Navigate to the project folder first:**
   ```powershell
   cd C:\Users\seren\lisagarbe.github.io
   ```
   Replace the path above with your actual project folder path on your computer.

3. **Then run Hugo:**
   ```powershell
   C:\Users\seren\AppData\Roaming\Hugo\0.154.2\hugo.exe
   ```
   Replace the path above with your actual Hugo path on your computer.
   
   This creates the `public/` folder with website files.

   **Important:** You must be in the project folder when running this command, otherwise Hugo won't find the config files.

### Step 2: Push to GitHub

**Make sure you're still in the project folder:**
```powershell
cd C:\Users\seren\lisagarbe.github.io
```
Replace the path above with your actual project folder path.

1. **Add changes:**
   ```powershell
   git add .
   ```

2. **Commit:**
   ```powershell
   git commit -m "Update website"
   ```

3. **Push:**
   ```powershell
   git push
   ```

**Note:** You can also use GitHub Desktop for Step 2 (pushing to GitHub) if you prefer a graphical interface, but Step 1 (building the site) must be done in PowerShell.

### Step 3: Wait for Deployment

- GitHub Pages will automatically update your site
- Changes appear within 1-5 minutes
- Check: `https://lisagarbe.github.io/`
