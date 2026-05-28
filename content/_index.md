---
title: ''
summary: ''
date: 2026-05-01
type: landing

sections:
  # ─────────────────────────────────────────────
  # 1. Hero biography
  # ─────────────────────────────────────────────
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
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

  # ─────────────────────────────────────────────
  # 2. Research focus — speaks to both audiences
  # ─────────────────────────────────────────────
  - block: markdown
    content:
      title: '🔬 Research'
      subtitle: 'Making VLMs that run on your phone — and that we actually understand.'
      text: |-
        My lab works on two tightly coupled problems:

        **① VLM Edge-device Inference Acceleration.** Vision-Language Models
        are the next wave of consumer AI, but most of them are too heavy to
        run on phones, AR glasses, or robots. We design model architectures,
        quantization schemes, KV-cache strategies, and NPU-GPU heterogeneous
        runtimes that make VLMs fast and energy-efficient on-device — building
        on hard-won experience shipping M-DLSS 3.0 to millions of HONOR users.

        **② VLM Interpretability.** As VLMs make more decisions inside
        consumer devices and embodied systems, knowing *why* they do what
        they do becomes a safety, trust, and product requirement. We study
        attention attribution, neuron-level concept localization, and
        failure-mode discovery for multimodal models.

        Together, these two directions answer a question we think will
        define the next decade of edge AI: **how do we make small, fast,
        trustworthy VLMs that real users want to live with?**
    design:
      columns: '1'

  # ─────────────────────────────────────────────
  # 3. For students — lab recruiting (anchor: #lab)
  # ─────────────────────────────────────────────
  - block: markdown
    id: lab
    content:
      title: '🎓 Join the Lab'
      subtitle: 'I want my students to win the future they want — and I will give everything I have to help them get there.'
      text: |-
        **The lab is open year-round to interns**, and we have **master's
        student slots** through Shenzhen University.

        I do not believe in students working *for* an advisor. I believe in
        students and advisors growing *together*. What I commit to every
        person who joins this group:

        - **A real research problem with real stakes.** Not toy benchmarks.
          You will work on things that matter for shipped products and for
          the frontier of VLM research.
        - **First-author papers + industry exposure.** Our work targets
          ICCV/ECCV/ACM MM/NeurIPS, and through our collaborations you
          will also see how research turns into products inside Google,
          Qualcomm, Alibaba, and HONOR.
        - **Career investment.** Whether you want to go to a top PhD program,
          a frontier industry lab, or start your own company — I will spend
          real time helping you get there. Your future is the project.
        - **Compute, mentorship, and respect.** Good GPUs. Weekly 1:1s.
          No silent treatment, no playing politics.

        If you are an undergraduate, master's, or industry engineer who
        wants to work on edge VLMs or interpretability, **please email me
        with your CV and a short note on what you want to build**. I read
        every message.

        > 我会竭力培养学生想要的未来,与学生的未来一起进步。
    design:
      columns: '1'
      css_class: 'border-l-4 border-primary-500 pl-6'

  # ─────────────────────────────────────────────
  # 4. For investors / industry partners
  # ─────────────────────────────────────────────
  - block: markdown
    id: partners
    content:
      title: '🤝 Industry Collaborations'
      subtitle: 'Research that ships.'
      text: |-
        During my time at HONOR Device (2024 – 2026), I worked in close
        collaboration with the AI teams at:

        - **Google** — Gemma open-model team
        - **Qualcomm** — on-device inference and NPU acceleration
        - **Alibaba** — Qwen (Tongyi Qianwen) Lab

        And shipped **M-DLSS 3.0**, the industry's first NPU-GPU
        heterogeneous frame interpolation system, to HONOR gaming phones —
        proving that frontier research can move from paper to consumer
        device in months, not years.

        **I am open to research collaborations, advisory engagements, and
        joint-lab arrangements** with companies and investors building in
        edge AI, on-device VLMs, embodied intelligence, and AI agents.
        Please reach out via email.
    design:
      columns: '1'

  # ─────────────────────────────────────────────
  # 5. Featured publications
  # ─────────────────────────────────────────────
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

  # ─────────────────────────────────────────────
  # 6. All publications
  # ─────────────────────────────────────────────
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation

  # ─────────────────────────────────────────────
  # 7. News
  # ─────────────────────────────────────────────
  - block: collection
    id: news
    content:
      title: News
      subtitle: ''
      text: ''
      page_type: blog
      count: 5
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      offset: 0
      order: desc
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]

  # ─────────────────────────────────────────────
  # 8. Contact CTA
  # ─────────────────────────────────────────────
  - block: cta-card
    content:
      title: 📩 Get in touch
      text: |-
        **Prospective students** — send your CV and what you want to build.

        **Industry & investors** — let's talk about edge VLMs, on-device
        agents, and where this is all going.
      button:
        text: Email me
        url: mailto:niuzehai@szu.edu.cn
    design:
      card:
        css_class: 'bg-gradient-to-br from-primary-500 via-primary-600 to-secondary-600 text-white shadow-2xl'
        css_style: ''
---
