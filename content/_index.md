---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '4rem'
  background:
    image:
      filename: background2.jpg

sections:
  - block: resume-biography
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: 
      # Show a call-to-action button under your biography? (optional)
      headings:
        about: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: small # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: 'About Me'
      subtitle: ''
      text: |-
        I work in the Holzapfel Lab on the South Pole Telescope experiment and am a member of the SPT-3G, SPT-3G+, and SPO (South Pole Observatory) collaborations. My PhD work has focused on improving CMB constraints on early-universe fundamental physics, ranging from polarized atmospheric mitigation to axion constraints. I am currently focused on instrumentation for SPT-3G+, the next-generation SPT receiver and "B-mode delensing machine." More information about each of these projects can be found below.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Projects
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Selected Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
 
---
