---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About Me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
#  - block: skills
#    content:
#      title: Skills
#      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
#      username: admin
#    design:
#      columns: '1'
  - block: collection
    id: news
    content:
      title: News
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      # default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      # buttons:
      #   - name: All
      #     tag: '*'
      #   - name: Deep Learning
      #     tag: Deep Learning
      #   - name: Other
      #     tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: true
  - block: collection
    id: publications
    content:
      title: Publications
      text: |-
        {{% callout note %}}
        You can quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      columns: '2'
      view: compact
  - block: collection
    id: notes
    content:
      title: Notes
      subtitle: ''
      text: |-
        Notes on selected topics in theoretical chemistry.
      filters:
        folders:
          - notes
    design:
      columns: '2'
      view: citation
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Feel free to contact me. Get in touch!
      # Contact (add or remove contact options as necessary)
      email: ziqiw@sas.upenn.edu
      phone: +1 (267) 366-2450
      # appointment_url: 'https://calendly.com'
      address:
        street: 231 South 34th Street
        city: Philadelphia
        region: PA
        postcode: '19104'
        country: United States
        country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '39.9507421'
        longitude: '-75.1947649'  
      contact_links:
       - icon: instagram
         icon_pack: fab
         name: Follow me on Ins
         link: 'https://www.instagram.com/altheorist'
      #  - icon: skype
      #    icon_pack: fab
      #    name: Skype Me
      #    link: 'skype:echo123?call'
      #  - icon: video
      #    icon_pack: fas
      #    name: Zoom Me
      #    link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
          # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
---
