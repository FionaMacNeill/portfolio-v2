---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: fiona
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: fiona
    design:
      columns: '1' 

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event 

  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2' 

  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'

  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Design
          tag: Design
        - name: Research
          tag: Research
 
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false

  - block: contact
    id: contact
    content:
      title: Contact
      email: hello@fionamacneill.co.uk 
      contact_links:
        - icon: mastodon
          icon_pack: fab
          name: '@fmacneill@toot.community'
          link: 'https://toot.community/@fmacneill'
        
      # Automatically link email and phone or display as text?
      autolink: true
  
    design:
      columns: '2' 

  #- block: markdown 
  #  id: gallery
  #  content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="work" >}} 
  #  design:
  #     columns: '1' 
---
<div id="wcb" class="carbonbadge"></div>
<script src="https://unpkg.com/website-carbon-badges@1.1.3/b.min.js" defer></script>