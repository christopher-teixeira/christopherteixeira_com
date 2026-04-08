---
# Leave the homepage title empty to use the site title
title: ""
date: 2026-04-06
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: resume-biography
    content:
      username: me
      text: ''
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: false
      name:
        size: md # Options: xs, sm, md, lg (default), xl
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded

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
              level: expert
            - name: Python
              icon: brands/python
              level: advanced
            - name: SQL
              icon: hero/circle-stack
              level: expert
            - name: SAS
              icon: custom/sas-svgrepo-com
              level: intermediate
        - name: "Data Manipulation & Analysis"
          items:
            - name: dplyr
              icon: brands/tidyverse
              level: expert
            - name: pandas
              icon: brands/pandas
              level: advanced
            - name: PostgreSQL
              icon: brands/postgresql
              level: advanced
            - name: Neo4J
              icon: brands/neo4j
              level: intermediate
        - name: "Data Visualization"
          items: 
            - name: ggplot2
              icon: brands/tidyverse
              level: expert
            - name: Shiny
              icon: brands/tidyverse
              level: advanced
            - name: Streamlit
              icon: brands/streamlit
              level: intermediate
            - name: Plotly
              icon: brands/plotly
              level: intermediate
            - name: Tableau
              icon: brands/tableau
              level: expert
    design: 
      show_levels: false # levels are 'expert', 'advanced', 'intermediate', 'beginner'
  - block: resume-experience
    id: experience
    content:
      username: me
      title: "Experience"
    design: 
      date_format: 'January 2006'
      is_education_first: true
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
      view: article-grid
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

---