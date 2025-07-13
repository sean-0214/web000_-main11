# Asset Management Guide for Hugo Blox Website

This guide provides systematic instructions for managing images and resource links for all content blocks in your Hugo Blox website. Follow these instructions to ensure consistent formatting and proper asset management across all sections.

## Directory Structure for Images

Every content type in Hugo Blox follows this pattern:
```
content/
├── section-name/
│   ├── entry-name/
│   │   ├── index.md       # Content file with front matter
│   │   ├── featured.jpg   # Main image (REQUIRED)
│   │   ├── gallery/       # Optional additional images
│   │   └── resources/     # Optional documents and downloadable files
```

## Standard Image Requirements

1. **Featured Images**:
   - **Filename**: Always use `featured.jpg` or `featured.png`
   - **Location**: Same directory as the `index.md` file
   - **Size**: Recommended 1200×800 pixels (3:2 aspect ratio)
   - **Format**: JPG or PNG (JPG preferred for photographs, PNG for graphics with transparency)
   - **File size**: Keep under 500KB for optimal performance

2. **Gallery Images** (optional):
   - Create a `gallery` subfolder and place additional images there
   - Use descriptive filenames: `image1.jpg`, `image2.jpg`, etc.
   - Maintain consistent dimensions for all gallery images

## Resource Links Structure

Every content block should include a standardized set of resource links using this format in the front matter:

```yaml
links:
  - name: Custom Link Title
    url: http://example.org/link-to-resource

url_pdf: http://example.org/paper.pdf       # Link to PDF version
url_code: https://github.com/sean-0214/repo   # Link to code repository
url_dataset: https://example.org/dataset     # Link to dataset
url_poster: https://example.org/poster.pdf   # Link to research poster
url_project: https://example.org/project     # Link to project website
url_slides: https://example.org/slides.pdf   # Link to presentation slides
url_source: https://example.org/source       # Link to source document
url_video: https://youtube.com/watch?v=ID    # Link to video presentation
```

## Systematic Upload Process for Each Section

### 1. Papers/Publications Section

For each publication in `content/publication/[publication-name]/`:

1. Prepare a featured image (1200×800px) named `featured.jpg`
2. Update the front matter in `index.md` with all resource links
3. Add the citation file if applicable (`cite.bib`)
4. Create a `resources` folder for supplementary materials if needed

### 2. Projects Section

For each project in `content/project/[project-name]/`:

1. Prepare a featured image (1200×800px) named `featured.jpg`
2. Update the front matter in `index.md` with all resource links
3. Add screenshots to `gallery/` folder if applicable
4. Create a `resources` folder for downloadable project files

### 3. Notes Section (formerly Teaching)

For each note in `content/notes/[note-name]/`:

1. Prepare a featured image (1200×800px) named `featured.jpg`
2. Update the front matter in `index.md` with all resource links
3. Add supplementary materials to a `resources` folder

## Example Implementation Process

1. **Gather Assets**:
   - Collect all images, PDFs, and other resources
   - Resize and optimize images to recommended specifications
   - Organize files by content type

2. **Prepare Directories**:
   - Create the appropriate directory structure for each section
   - Follow the naming conventions exactly

3. **Upload Files**:
   - Add `featured.jpg` to each content directory
   - Add additional resources to appropriate subfolders
   - Update all resource links in the front matter

4. **Verify Links**:
   - Test all links to ensure they're working
   - Validate image display across different sections

## Template Examples

### Publication Template

```yaml
---
title: "Publication Title"
authors:
- admin
date: "2023-01-01T00:00:00Z"
doi: ""

# Publication type (article-journal, paper-conference, etc.)
publication_types: ["article-journal"]

# Publication details
publication: "Journal Name"
publication_short: ""

abstract: "Abstract text goes here."
summary: "Brief summary for display in cards."

tags:
- Tag1
- Tag2

featured: true

links:
- name: Custom Link
  url: http://example.org

# Resource URLs - Replace '#' with actual URLs or leave as '#' if not applicable
url_pdf: http://example.org/paper.pdf
url_code: https://github.com/sean-0214/repo
url_dataset: https://example.org/dataset
url_poster: https://example.org/poster.pdf
url_project: https://example.org/project
url_slides: https://example.org/slides.pdf
url_source: https://example.org/source
url_video: https://youtube.com/watch?v=ID

# Featured image
image:
  caption: 'Image caption'
  focal_point: "Center"
  preview_only: false
---
```

### Project Template

```yaml
---
title: "Project Title"
summary: "Brief project summary"
tags:
- Tag1
- Tag2

# Optional external URL
external_link: ""

# Featured image
image:
  caption: Project image
  focal_point: Smart
  filename: featured.jpg

# Links
links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/username
  
# Resource URLs - Replace '#' with actual URLs or leave as '#' if not applicable
url_code: https://github.com/sean-0214/repo
url_pdf: https://example.org/whitepaper.pdf
url_slides: https://example.org/slides.pdf
url_video: https://youtube.com/watch?v=ID
---
```

### Note Template (formerly Teaching)

```yaml
---
title: "Note Title"
summary: "Brief summary of the note/resource"
date: "2023-01-01T00:00:00Z"

# Optional external URL
external_link: ""

# Featured image
image:
  caption: Resource image
  focal_point: Smart
  filename: featured.jpg

# Links
links:
- name: Download
  url: https://example.org/download
  icon_pack: fas
  icon: download

# Resource URLs - Replace '#' with actual URLs or leave as '#' if not applicable
url_code: https://github.com/sean-0214/repo
url_pdf: https://example.org/notes.pdf
url_slides: https://example.org/slides.pdf
url_video: https://youtube.com/watch?v=ID
---
```

## Bulk Asset Processing Tips

For processing multiple images at once:
1. Use batch processing tools like ImageMagick or Adobe Bridge
2. Create a script to rename files consistently
3. Consider using file organization software to maintain the directory structure

By following these guidelines, you'll ensure consistent presentation and functionality across all content blocks on your website.
