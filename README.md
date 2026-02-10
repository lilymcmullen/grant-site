# HDR Data Science Corps Grant Website

Main landing page and information hub for the NSF HDR Data Science Corps grant: **"Building Capacity in Data Science through Biodiversity, Conservation, and General Education"**

## About

A collaboration between:
- **University of Arizona** (Hispanic-Serving Institution, R1)
- **Lewis & Clark College** (Liberal Arts, Portland, OR)

This website serves as the central hub for all grant activities and materials.

## Website Structure

- **Overview**: Main landing page introducing the grant
- **About**: Detailed project description, intellectual merit, and broader impacts
- **Team**: Principal investigators, senior personnel, and collaborators
- **Program Components**:
  - AIM 1: Data in the Wild (links to separate course website)
  - AIM 2: Real-World Experiences
  - AIM 3: Faculty Professional Development
  - K-12 Outreach
- **Resources**: Publications, materials, and links

## Building the Site

This is a Quarto website. To build locally:

```bash
quarto preview
```

To render:

```bash
quarto render
```

## Deployment

The site is deployed via GitHub Pages from the `/docs` folder.

## Related Repositories

- [Data in the Wild - UA Track](https://github.com/BiodiversityDataScienceCorp/DataInTheWild_Website) - Computational emphasis course materials

## File Structure

```
grant-site/
├── index.qmd           # Main landing page
├── about.qmd           # Detailed grant description
├── team.qmd            # Project team and leadership
├── aim2.qmd            # AIM 2: Real-World Experiences
├── aim3.qmd            # AIM 3: Faculty Development
├── k12.qmd             # K-12 Outreach program
├── resources.qmd       # Publications and materials
├── _quarto.yml         # Site configuration
├── styles.scss         # Custom styling
└── images/             # Logos and images
    └── bdsc-logo-hex.png
```

## Design

The site uses the same clean, professional aesthetic as the Data in the Wild course website:

- **Fonts**: Vollkorn (headers), Raleway (body), Righteous (navbar)
- **Colors**: Dark blues and blanched almond matching BDSC branding
- **Layout**: Sidebar navigation with docked style

## Contributing

This project is part of an active NSF grant. For questions or collaboration inquiries, please contact us via [GitHub](https://github.com/BiodiversityDataScienceCorp).

## License

Materials developed under this grant follow FAIR principles and are shared openly for adaptation and use. Specific licensing information will be added as materials are published.

## Funding

This project is supported by the National Science Foundation under the Harnessing the Data Revolution (HDR) Data Science Corps (DSC) program, Grant Number [to be added].

## Contact

[BiodiversityDataScienceCorp on GitHub](https://github.com/BiodiversityDataScienceCorp)

---

**Last Updated**: December 2024
