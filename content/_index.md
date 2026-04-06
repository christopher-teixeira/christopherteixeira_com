---
# Leave the homepage title empty to use the site title
title: ""
date: 2026-04-06
type: landing

design:
  # Default section spacing
  spacing: "3rem"

sections:
  - block: resume-biography
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
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
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: resume-experience
    content:
      username: me
      title: "Experience"
    design: 
      date_format: 'January 2006'
      is_education_first: true

  # - block: cta-card
  #   content:
  #       title: test
  #       text: this is some text
  #       button: 
  #         text: test
  #       design:
  #         background:
  #           # Choose colors such as from https://html-color-codes.info
  #           gradient_start: '#4bb4e3'
  #           gradient_end: '#2b94c3'
  #           # The gradient angle from 0-360 degrees
  #           gradient_angle: 180
  #           # Text color (true=light, false=dark, or remove for the dynamic theme color).
  #           text_color_light: true
  # - block: features
  #   content: 
  #     title: test features
  #     text: this is some text
  #     items:
  #       - name: this is a name
  #         description: this is a description
  #         icon: custom/person-chalkboard-solid
  #       # - name: this is a name
  #       #   description: this is a description
  #       #   icon: custom/person-chalkboard-solid
  #       # - name: this is a name
  #       #   description: this is a description
  #       #   icon: custom/person-chalkboard-solid
  # - block: cta-button-list
  #   content:
  #     buttons:
  #       - text: Schedule a lecture
  #         icon: custom/person-chalkboard-solid
  #         url: https://calendar.app.google/GjvengVJdwvRCsXL6
        # - title: Watch my new YouTube video to achieve 20x productivity
        #   icon: custom/baseball-solid
        #   url: https://youtube.com
        # - title: Connect with me on LinkedIn
        #   icon: brands/linkedin
        #   url: https://linkedin.com
  # - block: resume-skills
  #   id: skills-old
  #   content: 
  #     title: Skills & Hobbies
  #     username: me
  #   design:
  #     show_skill_percentage: true
  - block: tech-stack
    id: skills
    content:
      title: "Tech Stack"
      subtitle: "Technologies I use to build things"
      categories: 
        - name: "Programming Languages"
          items: 
            - name: R
              icon: brands/r
            - name: Python
              icon: brands/python
            - name: SQL
              icon: hero/circle-stack
            - name: SAS
              icon: custom/sas-svgrepo-com
        - name: "Data Manipulation & Analysis"
          items:
            - name: dplyr
              icon: brands/tidyverse
            - name: pandas
              icon: brands/pandas
            - name: PostgreSQL
              icon: brands/postgresql
            - name: Neo4J
              icon: brands/neo4j
        - name: "Data Visualization"
          items: 
            - name: ggplot2
              icon: brands/tidyverse
            - name: Shiny
              icon: brands/tidyverse
            - name: Streamlit
              icon: brands/streamlit
            - name: Plotly
              icon: brands/plotly
            - name: Tableau
              icon: brands/tableau

  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      page_type: post
      count: 4
      filters:
        folders:
          - post
        author: ''
        category: ''
        tag: ''
        publication_type: ''
        featured_only: false
      offset: 0
      sort_by: 'Date'
      sort_ascending: false
    design:
      # Choose a layout view
      # view: date-title-summary
      view: article-grid
      # Reduce spacing
      # spacing:
      #   padding: [0, 0, 0, 0]
  # - block: collection
  #   id: projects
  #   content:
  #     title: Projects
  #     subtitle: ''
  #     text: 'This list of projects represents the details of my experience across my career and how I supported customers’ decision making on complex challenges.'
  #     count: 6
  #     filters:
  #       folders:
  #         - project
  #       author: ''
  #       category: ''
  #       tag: ''
  #       publication_type: ''
  #       featured_only: false
  #     offset: 0
  #     sort_by: 'Date'
  #     sort_ascending: false
  #   design:
  #     view: article-grid
  #     columns: 3

  - block: portfolio
    id: portfolio
    content:
      title: "Projects"
      subtitle: "This list of projects represents the details of my experience across my career and how I supported customers’ decision making on complex challenges."
      count: 6
      filters:
        folders:
          - project  # Or: research, portfolio, work, teaching, etc.
      buttons:
        - name: All
          tag: '*'
        - name: MITRE
          tag: MITRE
        - name: Epsilon
          tag: Epsilon
        - name: IBM
          tag: IBM
        - name: SAIC
          tag: SAIC
        - name: Other
          tag: Other
      default_button_index: 0
      archive:
        # Auto-shown if more items exist than displayed
        # Optionally customize:
        # enable: false  # Explicitly hide
        # link: "/work/"  # Custom URL
        # text: "Browse All"  # Custom text
    design:
      columns: 3
      fallback_icon: code-bracket  # Or: academic-cap, paint-brush, camera, etc.
      
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: card
      columns: 1
  # - block: stats
  #   id: stats
  #   content:
  #     title: test stats
  #     text: this is a section on stats
  #     items:
  #       - statistic: test stat 1
  #         description: test description for stat 1
  #       - statistic: test stat 2
  #         description: test description for stat 2
  #       - statistic: test stat 3
  #         description: test description for stat 3
---