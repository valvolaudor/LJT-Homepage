---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am Junteng Liu, a first-year PhD candidate at the [HKUST NLP Group](https://hkust-nlp.github.io/), supervised by [Professor Junxian He](https://jxhe.github.io/). I graduated from Shanghai Jiao Tong University (SJTU) in June 2024, where I was also previously advised by Professor Junxian He during my undergraduate studies.

My research focuses on natural language processing and machine learning, with a particular emphasis on building more capable, reliable, and interpretable large language models.

Research Interests
======
- **LLM Reasoning and Reinforcement Learning** — studying how to teach models to reason and improving reasoning quality with RL
- **Hallucination in Vision-Language Models (VLM)** — understanding and mitigating hallucination, especially in chart understanding
- **LLM Truthfulness and Interpretability** — exploring what lies inside LLMs and how to make them truthful

Education
======
- **Ph.D. in Computer Science** (2024–Present), Hong Kong University of Science and Technology
- **B.Eng.** (2020–2024), Shanghai Jiao Tong University

Research Experience
======
- **Research Intern** (February 2025 – Present), MINIMAX
- **Research Intern** (June 2024 – September 2024), Tencent WXG, advised by Zifei Shan
- **Research Intern** (June 2023 – December 2023), Shanghai AI Lab, advised by Prof. Yu Cheng

Skills
======
- **Programming Languages:** Python
- **Machine Learning / NLP Frameworks:** PyTorch, Hugging Face Transformers
- **Research Areas:** Large Language Models, Vision-Language Models, Reinforcement Learning, Reasoning, Hallucination, Truthfulness, Interpretability
- **Development Tools:** Git, Linux, Jupyter

Publications
======

{% include base_path %}

{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        **{{ category[1].title }}**
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

You can also view all publications on the [dedicated publications page](/publications/) or on my [Google Scholar profile](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate).

Awards
======
- Zhiyuan Honor Scholarship, Shanghai Jiao Tong University

Contact
======
- **Email:** [jliugi@connect.ust.hk](mailto:jliugi@connect.ust.hk)
- **GitHub:** [Vicent0205](https://github.com/Vicent0205)
- **Google Scholar:** [Junteng Liu](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate)
- **X (Twitter):** [@junteng88716710](https://x.com/junteng88716710)
