---
title: ''
summary: ''
date: 2024-01-01
type: landing

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        url: /uploads/CV_SContreras.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
      show_read_time: false
      show_date: false
  - block: collection
    id: publications
    content:
      title: Publications
      text: ''
      count: 0
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: collaborators
    content:
      title: External collaborators
      filters:
        folders:
          - collaborators
    design:
      view: article-grid
      fill_image: true
      columns: 4
      show_date: false
      show_read_time: false
      show_read_more: false
  - block: contact-info
    id: contact
    content:
      title: Contact
      subtitle: ''
      visit_title: Where to find me
      connect_title: Get in touch
      address:
        lines:
          - International Research Center for Complexity Sciences
          - Hangzhou International Innovation Institute (H3I), Beihang University
          - Hangzhou, China
      email: contreras@buaa.edu.cn
      social:
        - icon: academicons/google-scholar
          url: https://scholar.google.com/citations?user=OuIoqBIAAAAJ&hl=en
        - icon: academicons/orcid
          url: https://orcid.org/0000-0001-8909-774X
        - icon: brands/github
          url: https://github.com/seba-contreras
      show_form: false
---
