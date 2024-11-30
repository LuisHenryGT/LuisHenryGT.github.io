---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "5rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: resume-experience
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: true
  - block: collection
    id: papers
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: resume-awards
    id: certifications
    content:
      title: Certifications
      username: admin
  - block: resume-skills
    content:
      title: Skills & Hobbies
      username: admin
    design:
      show_skill_percentage: false
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming events by MRIG
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: resume-languages
    content:
      title: Languages
      username: admin
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - abs
        exclude_featured: false
---
