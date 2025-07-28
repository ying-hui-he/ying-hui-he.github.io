---
title: "LongProc: Benchmarking Long-Context Language Models on Long Procedural Generation"
collection: publications
category: conferences
permalink: /publication/longproc
citation: "Xi Ye, Fangcong Yin*, <b>Yinghui He*</b>, Joie Zhang*, Howard Yen*, Tianyu Gao, Greg Durrett, Danqi Chen
" # I've changed it to author
# teaser: "hi-tom.jpg"
excerpt: "“🤔Now most LLMs have >= 128K context sizes, but are they good at generating long outputs, such as writing 8K token chain-of-thought for a planning problem？ 
🔔Introducing LongProc (Long Procedural Generation), a new benchmark with 6 diverse tasks that challenge LLMs to synthesize highly dispersed information and generate long, structured outputs."
date: 2025-01-09
venue: "COLM 2025"
# slidesurl: "https://lit.eecs.umich.edu/Hi-ToM/"
paperurl: "https://arxiv.org/abs/2501.05414"
---

<figure>
  <img src="{{ site.baseurl }}/images/tom-wide.png" alt="Hi-ToM Figure 1">
</figure>

**_Abstract_**: Existing benchmarks for evaluating long-context language models (LCLMs) primarily focus on long-context recall, requiring models to produce short responses based on a few critical snippets while processing thousands of irrelevant tokens. We introduce LongProc (Long Procedural Generation), a new benchmark that requires both the integration of highly dispersed information and long-form generation. LongProc consists of six diverse procedural generation tasks, such as extracting structured information from HTML pages into a TSV format and executing complex search procedures to create travel plans. These tasks challenge LCLMs by testing their ability to follow detailed procedural instructions, synthesize and reason over dispersed information, and generate structured, long-form outputs (up to 8K tokens). Furthermore, as these tasks adhere to deterministic procedures and yield structured outputs, they enable reliable rule-based evaluation. We evaluate 17 LCLMs on LongProc across three difficulty levels, with maximum numbers of output tokens set at 500, 2K, and 8K. Notably, while all tested models claim a context window size above 32K tokens, open-weight models typically falter on 2K-token tasks, and closed-source models like GPT-4o show significant degradation on 8K-token tasks. Further analysis reveals that LCLMs struggle to maintain long-range coherence in long-form generations. These findings highlight critical limitations in current LCLMs and suggest substantial room for improvement.
