# Academic Website Template

A clean, responsive Jekyll-based template for academic personal websites. This template is designed for researchers, postdocs, and faculty members to showcase their research, publications, and professional information.

## Features

- Responsive design that works on desktop and mobile
- Publication management with separate sections for published papers and preprints
- Automatic CV integration
- Contact form integration via Formspree
- Clean, professional layout focused on research and academic content
- Easy configuration through YAML files

## Quick Start

### 1. Fork and Clone

1. Go to https://github.com/edwinlock/edwinlock.com and fork the repository
2. Rename your forked repository to `<yourusername>.github.io` or `<yourdomain.com>`
3. Update the repository description to reflect your site
4. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/<yourusername>/<repository-name>.git
   cd <repository-name>
   ```

### 2. Enable GitHub Pages

1. Go to your repository Settings
2. Navigate to the "Pages" section
3. Under "Source", select the branch you want to deploy (usually `main` or `jekyll`)
4. Save the settings

### 3. Configure Your Site

Open `_config.yml` and update the following fields:

```yaml
url: "https://www.yourdomain.com"  # IMPORTANT: Must include https://

fullname: Your Full Name
position: Your Position (e.g., "Lecturer", "Postdoctoral Researcher")
department: Your Department
university: Your University

# Optional address fields
building: Building Name
street: Street Address
city: City
postcode: Postal Code
country: Country

email: your.email@domain.com
secondary: alternative.email@domain.com  # optional

formurl: https://formspree.io/yourformid  # For contact form
```

### 4. Customize Your Content

#### Update Your Profile
- Edit `index.md` to add your bio, research interests, and about section
- Replace `profile.png` with your own profile photo

#### Add Publications
Publications are managed through YAML files:
- `_data/publications.yml` - For published papers
- `_data/preprints.yml` - For preprints and working papers

Example publication entry:
```yaml
- title: "Your Paper Title"
  authors: "Author1, Author2, Author3"
  venue: "Conference/Journal Name"
  year: 2024
  pdf: "pdfs/paper.pdf"  # optional
  link: "https://doi.org/..."  # optional
```

#### Update Your CV
- Place your CV PDF in the `pdfs/` directory as `cv.pdf`
- Or update the link in `index.md` to point to your CV location

### 5. Custom Domain (Optional)

If using a custom domain:
1. Create or update the `CNAME` file with your domain name (e.g., `www.yourdomain.com`)
2. Configure DNS settings with your domain provider to point to GitHub Pages
3. Update the `url` field in `_config.yml` to match your custom domain

If using GitHub Pages default domain (`<username>.github.io`):
1. Delete the `CNAME` file
2. Update `url` in `_config.yml` to `https://<username>.github.io`

### 6. Deploy

```bash
git add .
git commit -m "Customize site with my information"
git push origin main
```

Your site should be live at your GitHub Pages URL within a few minutes!

## Local Development

To test your site locally before deploying:

1. Install Jekyll and dependencies:
   ```bash
   gem install bundler jekyll
   bundle install
   ```

2. Run the local server:
   ```bash
   bundle exec jekyll serve
   ```

3. View your site at `http://localhost:4000`

## Project Structure

```
.
├── _config.yml           # Main configuration file
├── _data/
│   ├── publications.yml  # Published papers
│   └── preprints.yml     # Preprints and working papers
├── _layouts/             # Page templates
├── _includes/            # Reusable components
├── index.md              # Home page content
├── research.html         # Research/publications page
├── pdfs/                 # PDF files (CV, papers)
│   └── cv.pdf
└── profile.png           # Profile photo
```

## Support

For issues or questions about this template, please open an issue on the GitHub repository.

## License

Feel free to fork and customize this template for your own academic website.
