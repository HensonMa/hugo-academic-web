---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  # - block: features
  #   content:
  #     title: Skills
  #     items:
  #       - name: R
  #         description: 90%
  #         icon: r-project
  #         icon_pack: fab
  #       - name: Statistics
  #         description: 100%
  #         icon: chart-line
  #         icon_pack: fas
  #       - name: Photography
  #         description: 10%
  #         icon: camera-retro
  #         icon_pack: fas
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Software Engineering at Machine Learning Platform
          company: Intel Cooperation
          company_url: ''
          company_logo: intel-logo
          location: Shanghai, China
          date_start: '2022-12-19'
          date_end: '2022-06-08'
          description: |2-
              * Maintained backend support of Intel’s BigDL-Nano to provide acceleration for PyTorch and TensorFlow programs.
              * Applied Intel Arc series GPU support and Intel’s BigDL-Nano framework tools to accelerate Stable Diffusion’s inferencing on frontend client platform.
              * Added quantization support for large language models (LLMs, including ChatGLM, GPT, and LLaMA) to reduce their inference time.
              * Benchmarked LLM’s performance on distributed clusters by using Intel’s BigDL-Orca.
              * Supported GitHub CI/CD actions for Intel’s BigDL-LLM new package development.
        - title: Research Assistant
          company: Cornell University
          company_url: ''
          company_logo: cornell
          location: Ithaca, NY
          date_start: '2022-03-02'
          date_end: '2022-09-02'
          description: |2-
              * Analyzed PokeBNN’s inference process by breaking down the overall inference time into partial latencies of high-level functional abstractions and low-level TFLite atomic graph operations using Larq benchmarking methods.
              * Reduced the inference time of PokeBNN on embedded processors by 61.54% by replacing heavy Shortcuts and Activation functions with alternative TensorFlow and Larq efficient MLOps.
              * Designed two-phase CIFAR10 training of PokeBNN with modified structures using CUDA, obtaining the best validation accuracy of 87.94%.
        - title: Research Assistant
          company: John Hopcroft Center, Shanghai Jiao Tong University
          company_url: 'https://jhc.sjtu.edu.cn/'
          company_logo: SJTU
          location: Shanghai, China
          date_start: '2021-09-02'
          date_end: '2022-09-02'
          description: |2-
              * Trained neural networks to lower the interaction order among input variables to improve their adversarial robustness.
              * Generated adversarial image samples from back-propagation of PGD-20 attack on adversarial-trained ResNet18.
              * Added untrained regional fully-connected layers implemented by PyTorch modules to do classification task in training, which yields 73.2% improvement on the adversarial robustness of ResNet18 compared with the original one.
              * Designed a new loss function based on Hessian matrix to lower the high-order gradient influence between different regions of feature maps in neural networks.
        - title: Research Assistant
          company: DCE Lab, Shanghai Jiao Tong University
          company_url: 'https://en.sjtu.edu.cn/'
          company_logo: SJTU
          location: Shanghai, China
          date_start: '2021-01-02'
          date_end: '2021-08-02'
          description: |2-
              * Analyzed annual data from COSCO SHIPPING Lines by Correlation Analysis and Principal Component Analysis to extract important features using Pandas and NumPy.
              * Built a new time-series model [Long-short Term Memory framework with Empirical Mode Decomposition and Attention mechanism] using TensorFlow Keras to help predict daily shipment prices and market demands, which reduced the error rate by 52.31% on average compared to the baseline model RNN.
    design:
      columns: '2'
  # - block: accomplishments
  #   content:
  #     # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
  #     title: 'Accomplish&shy;ments'
  #     subtitle:
  #     # Date format: https://wowchemy.com/docs/customization/#date-format
  #     date_format: Jan 2006
  #     # Accomplishments.
  #     #   Add/remove as many `item` blocks below as you like.
  #     #   `title`, `organization`, and `date_start` are the required parameters.
  #     #   Leave other parameters empty if not required.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - certificate_url: https://www.coursera.org
  #         date_end: ''
  #         date_start: '2021-01-25'
  #         description: ''
  #         organization: Coursera
  #         organization_url: https://www.coursera.org
  #         title: Neural Networks and Deep Learning
  #         url: ''
  #       - certificate_url: https://www.edx.org
  #         date_end: ''
  #         date_start: '2021-01-01'
  #         description: Formulated informed blockchain models, hypotheses, and use cases.
  #         organization: edX
  #         organization_url: https://www.edx.org
  #         title: Blockchain Fundamentals
  #         url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
  #       - certificate_url: https://www.datacamp.com
  #         date_end: '2020-12-21'
  #         date_start: '2020-07-01'
  #         description: ''
  #         organization: DataCamp
  #         organization_url: https://www.datacamp.com
  #         title: 'Object-Oriented Programming in R'
  #         url: ''
  #   design:
  #     columns: '2'
  # - block: collection
  #   id: posts
  #   content:
  #     title: Recent Posts
  #     subtitle: ''
  #     text: ''
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       folders:
  #         - post
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: compact
  #     columns: '2'
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
        - name: System
          tag: system
        - name: Video Game
          tag: game
        - name: Others
          tag: other
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="mpc" >}}
    design:
      columns: '1'
  # - block: collection
  #   id: featured
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     columns: '2'
  #     view: card
  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: |-
  #       {{% callout note %}}
  #       Quickly discover relevant content by [filtering publications](./publication/).
  #       {{% /callout %}}
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: true
  #   design:
  #     columns: '2'
  #     view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Please contact me through ways below if you're interested.  
      # Contact (add or remove contact options as necessary)
      email: pima@ucsd.edu
      # phone: 888 888 88 88
      # appointment_url: 'https://calendly.com'
      address:
        street: 9500 Gilman Drive
        city: La Jolla
        region: CA
        postcode: '92093'
        country: United States
        country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/HesensMa'
        # - icon: skype
        #   icon_pack: fab
        #   name: Skype Me
        #   link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   # formspree:
      #   #   id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: true
    design:
      columns: '2'
---
