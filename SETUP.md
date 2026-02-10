# Setup Instructions for Grant Website

## Quick Start

1. **Create a new GitHub repository** named something like:
   - `HDR-DSC-Grant`
   - `DataScienceCorps-Website`
   - `BDSC-Grant-Website`

2. **Clone the repository locally**:
   ```bash
   git clone git@github.com:BiodiversityDataScienceCorp/YOUR-REPO-NAME.git
   cd YOUR-REPO-NAME
   ```

3. **Add all the files** from the `grant-site` folder:
   - `index.qmd`
   - `about.qmd`
   - `team.qmd`
   - `aim2.qmd`
   - `aim3.qmd`
   - `k12.qmd`
   - `resources.qmd`
   - `_quarto.yml`
   - `styles.scss`
   - `.nojekyll`
   - `README.md`

4. **Create an `images` folder** and add your logo:
   ```bash
   mkdir images
   # Copy bdsc-logo-hex.png to images/
   ```

5. **Add a header image** (optional):
   - Find or create an image representing biodiversity/data science
   - Save it as `images/grant-header.jpg`
   - Or remove the image line from `index.qmd` if you don't want one

6. **Preview the site**:
   ```bash
   quarto preview
   ```

7. **Render the site**:
   ```bash
   quarto render
   ```

8. **Commit and push**:
   ```bash
   git add .
   git commit -m "Initial grant website"
   git push
   ```

9. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Set source to "Deploy from a branch"
   - Select `main` branch and `/docs` folder
   - Save

## Customization

### Update Award Number

In `index.qmd`, find and update:
```markdown
This project is supported by the National Science Foundation under the Harnessing the Data Revolution (HDR) Data Science Corps (DSC) program.
```

Add: `Grant Number [YOUR-NSF-AWARD-NUMBER]`

### Add Header Image (Optional)

If you want a header image on the landing page:
1. Add an appropriate image to `images/grant-header.jpg`
2. Keep the line in `index.qmd`: `![](images/grant-header.jpg){fig-alt="Biodiversity and data science"}`

If you don't want a header image:
1. Remove or comment out that line in `index.qmd`

### Update Links

When you have materials ready for AIMs 2, 3, or K-12:

In `_quarto.yml`, update the `href` from `aim2.qmd` to the actual URL:
```yaml
- text: "AIM 2: Real-World Experiences"
  href: https://link-to-aim2-site.github.io/
```

### Modify Colors (Optional)

To change the color scheme, edit `styles.scss`:
```scss
// Change these colors to match your branding
$dark-blue: #1E4557;
$blanched-almond: #FFEBCD;
$magenta: #8A1665;
```

## File Overview

| File | Purpose |
|------|---------|
| `index.qmd` | Main landing page with overview of all AIMs |
| `about.qmd` | Detailed grant description, intellectual merit, broader impacts |
| `team.qmd` | Project team, PIs, senior personnel, cores |
| `aim2.qmd` | Real-world internship experiences details |
| `aim3.qmd` | Faculty professional development program |
| `k12.qmd` | K-12 outreach through Bio/Diversity Project |
| `resources.qmd` | Publications, materials, external links |
| `_quarto.yml` | Site configuration and navigation |
| `styles.scss` | Custom styling matching Data in the Wild |

## Updating Content

All content is in `.qmd` (Quarto Markdown) files. To update:

1. Edit the relevant `.qmd` file
2. Preview changes: `quarto preview`
3. Render: `quarto render`
4. Commit and push to update live site

## Troubleshooting

**Site not updating on GitHub Pages?**
- Make sure you've rendered (`quarto render`) before pushing
- Check that GitHub Pages is pointing to `/docs` folder
- Wait a few minutes for GitHub to rebuild

**Preview not working?**
- Make sure Quarto is installed: `quarto --version`
- Check that all file paths are correct
- Ensure `images/bdsc-logo-hex.png` exists

**Styling looks wrong?**
- Verify `styles.scss` is in the root directory
- Check that `_quarto.yml` references `styles.scss` correctly
- Clear browser cache and refresh

## Next Steps

1. ✅ Create repository and add files
2. ✅ Preview locally to verify everything works
3. ✅ Add your logo and optional header image
4. ✅ Update NSF award number
5. ✅ Deploy to GitHub Pages
6. 🔄 Share URL with team for feedback
7. 🔄 Update content as materials become available

## Questions?

If you need help or want to make changes to the design, let me know!
