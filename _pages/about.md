---
permalink: /
title: "Yassine El Kheir"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
/* ---- Homepage styling ---- */
.intro-lead { font-size: 1.02em; line-height: 1.65; margin-bottom: 1.4em; }
.intro-lead .thread {
  display: inline-block;
  border-left: 3px solid #2563eb;
  background: #f1f5f9;
  padding: 0.55em 0.9em;
  margin-top: 0.6em;
  border-radius: 0 6px 6px 0;
  font-style: italic;
}

.hiring-banner {
  background: linear-gradient(90deg, #ecfdf5 0%, #f0fdf4 100%);
  border: 1px solid #bbf7d0;
  border-left: 4px solid #059669;
  padding: 0.7em 1em;
  border-radius: 6px;
  margin: 0.8em 0 1.4em 0;
  font-size: 0.95em;
}
.hiring-banner .pill {
  display: inline-block;
  background: #059669; color: white;
  padding: 1px 9px; border-radius: 999px;
  font-size: 0.75em; font-weight: 700;
  letter-spacing: 0.04em;
  margin-right: 8px;
  vertical-align: 1px;
}

.section-title {
  font-size: 1.18em;
  font-weight: 700;
  margin: 2.0em 0 0.8em 0;
  padding-bottom: 0.35em;
  border-bottom: 1px solid #e2e8f0;
  letter-spacing: 0.01em;
}

/* News */
.news-list { list-style: none; padding-left: 0; margin: 0; }
.news-list li {
  display: flex; gap: 0.9em;
  padding: 0.45em 0;
  border-bottom: 1px dashed #e5e7eb;
  font-size: 0.95em; line-height: 1.5;
}
.news-list li:last-child { border-bottom: none; }
.news-date {
  flex: 0 0 95px;
  font-variant-numeric: tabular-nums;
  color: #64748b;
  font-size: 0.88em;
  font-weight: 600;
  padding-top: 2px;
}
.news-body { flex: 1; }
.news-tag {
  display: inline-block;
  font-size: 0.72em;
  font-weight: 700;
  padding: 1px 7px;
  border-radius: 4px;
  margin-right: 6px;
  letter-spacing: 0.04em;
  vertical-align: 1px;
}
.tag-paper { background: #dbeafe; color: #1e3a8a; }
.tag-talk  { background: #fef3c7; color: #92400e; }
.tag-grant { background: #dcfce7; color: #166534; }
.tag-org   { background: #fce7f3; color: #9d174d; }
.tag-code  { background: #e0e7ff; color: #3730a3; }
.tag-visit { background: #f1f5f9; color: #334155; }

/* Project cards */
.proj-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(290px, 1fr));
  gap: 14px;
  margin: 0.6em 0 0.4em 0;
}
.proj-card {
  display: flex;
  gap: 14px;
  padding: 14px;
  border: 1px solid #e5e7eb;
  border-radius: 10px;
  background: #ffffff;
  transition: box-shadow 0.18s ease, transform 0.18s ease;
}
.proj-card:hover {
  box-shadow: 0 6px 18px rgba(15,23,42,0.08);
  transform: translateY(-1px);
}
.proj-logo {
  flex: 0 0 64px;
  width: 64px; height: 64px;
  border-radius: 10px;
  overflow: hidden;
  background: #ffffff;
  border: 1px solid #f1f5f9;
  display: flex; align-items: center; justify-content: center;
}
.proj-logo img { max-width: 86%; max-height: 86%; object-fit: contain; display: block; }
.proj-body { flex: 1; min-width: 0; }
.proj-title {
  font-weight: 700;
  font-size: 1.0em;
  margin: 0 0 2px 0;
  color: #0f172a;
}
.proj-meta {
  font-size: 0.78em;
  color: #64748b;
  margin-bottom: 6px;
  letter-spacing: 0.02em;
}
.proj-desc { font-size: 0.88em; line-height: 1.45; color: #334155; margin: 0 0 6px 0; }
.proj-links { font-size: 0.82em; }
.proj-links a {
  display: inline-block;
  margin-right: 8px;
  color: #2563eb;
  text-decoration: none;
}
.proj-links a:hover { text-decoration: underline; }

/* Publications inline */
.pub-list { padding-left: 0; list-style: none; }
.pub-list li {
  padding: 0.55em 0;
  border-bottom: 1px dashed #e5e7eb;
  font-size: 0.94em;
  line-height: 1.5;
}
.pub-list li:last-child { border-bottom: none; }
.pub-title { font-weight: 600; color: #0f172a; }
.pub-venue {
  display: inline-block;
  font-size: 0.74em;
  font-weight: 700;
  padding: 1px 7px;
  margin-right: 6px;
  background: #e0f2fe;
  color: #075985;
  border-radius: 4px;
  letter-spacing: 0.03em;
}
.pub-authors { font-size: 0.88em; color: #475569; }
.pub-authors .me { font-weight: 700; color: #0f172a; }

/* Talks list */
.talk-list { padding-left: 0; list-style: none; }
.talk-list li {
  padding: 0.4em 0;
  border-bottom: 1px dashed #e5e7eb;
  font-size: 0.93em;
  display: flex; gap: 0.9em;
}
.talk-list li:last-child { border-bottom: none; }
.talk-date {
  flex: 0 0 95px; color: #64748b; font-size: 0.85em; font-weight: 600;
  font-variant-numeric: tabular-nums; padding-top: 2px;
}
.talk-body { flex: 1; }

/* Experience timeline */
.exp-list { padding-left: 0; list-style: none; }
.exp-list li {
  display: flex; gap: 14px;
  padding: 0.7em 0;
  border-bottom: 1px dashed #e5e7eb;
}
.exp-list li:last-child { border-bottom: none; }
.exp-logo {
  flex: 0 0 56px; width: 56px; height: 56px;
  border-radius: 8px; overflow: hidden;
  background: #ffffff;
  border: 1px solid #f1f5f9;
  display: flex; align-items: center; justify-content: center;
}
.exp-logo img { max-width: 86%; max-height: 86%; object-fit: contain; }
.exp-body { flex: 1; font-size: 0.93em; }
.exp-role { font-weight: 700; color: #0f172a; }
.exp-where { color: #475569; }
.exp-when {
  color: #64748b; font-size: 0.84em; font-weight: 600;
  font-variant-numeric: tabular-nums;
}

/* Awards */
.award-list { padding-left: 0; list-style: none; }
.award-list li {
  padding: 0.35em 0;
  font-size: 0.94em;
}
.award-year {
  display: inline-block;
  font-variant-numeric: tabular-nums;
  font-weight: 700;
  color: #64748b;
  width: 56px;
}
</style>

<p class="intro-lead">
  I'm a PhD researcher at the 
  <a href="https://www.dfki.de/en/web">German Research Center for AI (DFKI)</a> 
  and <a href="https://www.tu.berlin/en/">TU Berlin</a>, advised by 
  <a href="https://scholar.google.de/citations?user=BC_qcg0AAAAJ">Prof. Sebastian Möller</a> 
  and <a href="https://scholar.google.de/citations?user=tImnUh0AAAAJ">Dr. Tim Polzehl</a>. 
  I also lead R&amp;D (part-time) at 
  <a href="https://gretchen-ai.com/">Gretchen AI</a> in Berlin.
  <br><br>
  My research sits at the intersection of 
  <b>speech foundation models</b>, <b>trustworthy audio AI</b>, and 
  <b>linguistic inclusivity</b>. I build and study systems that detect AI-generated 
  speech, interpret self-supervised representations, and extend the reach of 
  modern speech AI to languages and dialects that mainstream models leave behind — 
  with a focus on Arabic and its rich dialectal diversity.
  <br><br>
  Before Berlin, I spent two years at the 
  <a href="https://www.hbku.edu.qa/en/qcri">Qatar Computing Research Institute</a>, 
  contributing to <a href="https://arxiv.org/pdf/2501.13944">Fanar</a> 
  (Qatar's Arabic-centric LLM) and leading 
  <a href="https://arxiv.org/pdf/2305.07445">QVoice</a>, 
  the first end-to-end Arabic mispronunciation detection system.
  <br><br>
  <span class="thread">
    The question driving my work: <i>how do we make speech AI that is 
    <b>robust</b> enough to trust, <b>efficient</b> enough to deploy, 
    and <b>inclusive</b> enough to serve everyone?</i>
  </span>
</p>

<!-- <p class="intro-lead">
I'm a PhD researcher in <b>machine learning for speech and audio</b> at the <a href="https://www.dfki.de/en/web">German Research Center for AI (DFKI)</a> and <a href="https://www.tu.berlin/en/">TU Berlin</a>, advised by <a href="https://scholar.google.de/citations?user=BC_qcg0AAAAJ">Prof. Sebastian Möller</a> and <a href="https://scholar.google.de/citations?user=tImnUh0AAAAJ">Dr. Tim Polzehl</a>. I'm also Research &amp; Engineering Lead (part-time) at <a href="https://gretchen-ai.com/">Gretchen AI</a> in Berlin.
<br><br>
My work spans <b>speech and audio foundation models</b>, <b>audio language models</b>, <b>multilingual speech</b> (ASR, TTS, pronunciation, dialects), and <b>robust, trustworthy speech AI</b>, including deepfake detection and anti-spoofing. Before Berlin I spent two years as a Research Associate at <a href="https://www.hbku.edu.qa/en/qcri">Qatar Computing Research Institute</a>, where I contributed to <a href="https://arxiv.org/pdf/2501.13944">Fanar</a> (Arabic-centric LLM) and led <a href="https://arxiv.org/pdf/2305.07445">QVoice</a>, the first end-to-end Arabic mispronunciation detection system.
<br>
<span class="thread">The thread across my work: speech AI that is <b>robust</b> in adversarial settings, <b>efficient</b> enough to deploy, and <b>inclusive</b> of languages and dialects that mainstream foundation models leave behind.</span>
</p> -->

<div class="hiring-banner">
<span class="pill">OPEN</span>
<b>Looking for a research position starting January 2027.</b> Speech / audio ML, foundation models, audio LLMs, multilingual speech, or trust &amp; safety in audio. Industry or academia, Europe / Middle East / remote. <a href="mailto:yassine.el_kheir@dfki.de">Get in touch.</a>
</div>

<div class="section-title">🔬 Research Interests</div>

Interested in the science of robust speech intelligence, how foundation models represent, reason about, and are fooled by audio, and how to make them work across the world's linguistic diversity

- **Speech and audio foundation models**: SSL representations, audio LLMs, interpretability, efficient architectures
- **Multilingual and low-resource speech**: ASR, TTS, pronunciation assessment, dialectal modeling
- **Robust and trustworthy audio AI**: deepfake detection, anti-spoofing, generalization across unseen domains
- **Speech-language models**: joint reasoning over acoustic and semantic features, explainable predictions
- **Tokenization for multilingual LLMs**: morphology-aware methods (MorphBPE used in Fanar)

<div class="section-title">🚀 Flagship Projects</div>

<p style="font-size:0.93em; color:#475569; margin-top:-0.2em;">
Listed roughly newest-first. See the <a href="{{ '/projects/' | relative_url }}">Projects</a> page for the full picture.
</p>

<div class="proj-grid">

  <div class="proj-card">
    <div class="proj-logo"><img src="{{ '/images/projects/deepfense.png' | relative_url }}" alt="DeepFense"></div>
    <div class="proj-body">
      <div class="proj-title">DeepFense Framework</div>
      <div class="proj-meta">DFKI &middot; open-source &middot; arXiv 2026</div>
      <p class="proj-desc">Open-source, configuration-driven framework for deepfake audio detection research. Mix SSL frontends (Wav2Vec, WavLM, HuBERT, MERT, EAT), backends (AASIST, ECAPA, Nes2Net, RawNet2), losses and augmentations entirely via YAML. Ships with <b>455+ pretrained models</b> on HuggingFace.</p>
      <div class="proj-links">
        <a href="https://deepfense.github.io/">website</a>
        <a href="https://huggingface.co/DeepFense">🤗 models</a>
        <a href="https://github.com/Yaselley/deepfense-framework">code</a>
        <a href="https://arxiv.org/abs/2604.08450">paper</a>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-logo"><img src="{{ '/images/projects/atlasia.png' | relative_url }}" alt="AtlasIA"></div>
    <div class="proj-body">
      <div class="proj-title">AtlasIA, Open-Source AI for Morocco</div>
      <div class="proj-meta">Speech Team Lead &middot; 2025 to present</div>
      <p class="proj-desc">Leading the Speech Team to build open-source AI grounded in Moroccan linguistic identity. Built <b><a href="https://huggingface.co/blog/abdeljalilELmajjodi/moulsot">MoulSot</a></b>, a curated <b>80-hour Moroccan Darija ASR corpus</b> distilled from 1,500 hours of YouTube speech through a multi-stage pipeline (Silero VAD, SQUIM, Audiobox Aesthetics, DNS64, pyannote, Argilla, Gemini 2.5 Pro), and fine-tuned <b>Qwen3-ASR-1.7B</b> on top. Also building the first natural Text-to-Speech system and tokenizer for Moroccan Darija.</p>
      <div class="proj-links">
        <a href="https://atlasia.ma/">website</a>
        <a href="https://huggingface.co/atlasia">🤗 HuggingFace</a>
        <a href="https://huggingface.co/blog/abdeljalilELmajjodi/moulsot">MoulSot blog</a>
        <a href="https://huggingface.co/atlasia/moulsot.v0.3">model</a>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-logo"><img src="{{ '/images/projects/gretchen.svg' | relative_url }}" alt="Gretchen AI"></div>
    <div class="proj-body">
      <div class="proj-title">Gretchen AI</div>
      <div class="proj-meta">Research &amp; Engineering Lead (part-time) &middot; 2025 to present</div>
      <p class="proj-desc">Co-leading R&amp;D for generative-media detection at a Berlin startup. Built an image deepfake detector that ranked <b>#1 on the Deepfake-Eval 2024 benchmark</b> (~83% accuracy), and designed the production inference pipeline.</p>
      <div class="proj-links">
        <a href="https://gretchen-ai.com/">website</a>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-logo"><img src="{{ '/images/projects/newspolygraph.png' | relative_url }}" alt="News-Polygraph"></div>
    <div class="proj-body">
      <div class="proj-title">News-Polygraph and Mamba SSL line</div>
      <div class="proj-meta">DFKI &middot; Interspeech, WASPAA, NAACL 2025 &middot; ICASSP 2026</div>
      <p class="proj-desc">Speech contributions to <b>News-Polygraph</b>, a BMBF-funded multimodal disinformation platform. Includes <b>BiCrossMamba-ST</b> (one of the first Mamba-based anti-spoofing models, 28% fewer params), spectral plus SSL fusion, layer-wise SSL interpretability, and a parameter-efficient multi-scale adapter for synthetic speech detection (ICASSP 2026).</p>
      <div class="proj-links">
        <a href="https://arxiv.org/pdf/2505.13930">BiCrossMamba</a>
        <a href="https://arxiv.org/pdf/2507.20417">Two Views</a>
        <a href="https://arxiv.org/abs/2510.24852">Adapter</a>
        <a href="https://news-polygraph.com/">project</a>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-logo"><img src="{{ '/images/projects/iqraeval.png' | relative_url }}" alt="Iqra'Eval"></div>
    <div class="proj-body">
      <div class="proj-title">Iqra'Eval, Quranic Pronunciation</div>
      <div class="proj-meta">Founder &amp; Lead Organizer &middot; ArabicNLP 2025 &middot; IQRA 2026 Interspeech Challenge</div>
      <p class="proj-desc">A multi-institutional initiative benchmarking Arabic pronunciation assessment via Quranic recitation. Organized the first shared task at ArabicNLP 2025; second iteration accepted as an <b>Interspeech 2026 Challenge</b> expanding to general MSA. Co-built <b>QuranMB</b>, the first expert-annotated Quranic mispronunciation dataset.</p>
      <div class="proj-links">
        <a href="https://huggingface.co/IqraEval">🤗 dataset</a>
        <a href="https://arxiv.org/abs/2506.07757">paper</a>
        <a href="https://arxiv.org/abs/2603.29087">IQRA 2026</a>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-logo"><img src="{{ '/images/projects/fanar.svg' | relative_url }}" alt="Fanar"></div>
    <div class="proj-body">
      <div class="proj-title">Fanar and MorphBPE</div>
      <div class="proj-meta">QCRI &middot; 2022 to 2024</div>
      <p class="proj-desc">Contributed to <b>Fanar</b>, Qatar's Arabic-centric multimodal LLM. Designed <b>MorphBPE</b>, a morphology-aware tokenizer that improves fertility and downstream generation for morphologically rich languages. Helped run training pipelines from 300M to 3B parameters.</p>
      <div class="proj-links">
        <a href="https://arxiv.org/pdf/2501.13944">Fanar paper</a>
        <a href="https://arxiv.org/pdf/2502.00894">MorphBPE</a>
      </div>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-logo"><img src="{{ '/images/projects/qvoice.png' | relative_url }}" alt="QVoice"></div>
    <div class="proj-body">
      <div class="proj-title">QVoice and Arabic Speech Stack</div>
      <div class="proj-meta">QCRI &middot; Interspeech 2023 &middot; 6+ papers</div>
      <p class="proj-desc">Led <b>QVoice</b>, the first end-to-end mispronunciation detection system for MSA, plus a series of follow-on SOTA results on L2 speech assessment, multilingual MDD, augmentation (SpeechBlender), and the AraVoiceL2 dataset.</p>
      <div class="proj-links">
        <a href="https://arxiv.org/pdf/2305.07445">QVoice</a>
        <a href="https://arxiv.org/pdf/2310.13974">Review</a>
      </div>
    </div>
  </div>

</div>

<div class="section-title">📰 News</div>

<ul class="news-list">
  <li>
    <span class="news-date">2026-05</span>
    <span class="news-body"><span class="news-tag tag-talk">talk</span>Returning as <b>Speech ML mentor</b> and <b>PhD Students panelist</b> at <a href="https://hackai.ma">HackAI Morocco 2026</a>.</span>
  </li>
  <li>
    <span class="news-date">2026-05</span>
    <span class="news-body"><span class="news-tag tag-code">release</span>Released <b><a href="https://huggingface.co/blog/abdeljalilELmajjodi/moulsot">MoulSot</a></b>: 80 hours of curated Moroccan Darija ASR data distilled from 1,500h of YouTube, plus a fine-tuned Qwen3-ASR model (<a href="https://huggingface.co/atlasia/moulsot.v0.3">atlasia/moulsot.v0.3</a>).</span>
  </li>
  <li>
    <span class="news-date">2026-03</span>
    <span class="news-body"><span class="news-tag tag-paper">paper</span><b><a href="https://arxiv.org/abs/2604.08450">DeepFense</a></b> framework paper is out: a unified, modular, extensible toolkit for robust deepfake audio detection.</span>
  </li>
  <li>
    <span class="news-date">2026-02</span>
    <span class="news-body"><span class="news-tag tag-org">organize</span><b><a href="https://arxiv.org/abs/2603.29087">IQRA 2026</a></b>, the second Iqra'Eval, accepted as an <b>Interspeech 2026 Challenge</b> on MSA pronunciation assessment.</span>
  </li>
  <li>
    <span class="news-date">2026-01</span>
    <span class="news-body"><span class="news-tag tag-paper">paper</span><b>Two ICASSP 2026 papers</b> accepted: <a href="https://arxiv.org/abs/2510.24852">a parameter-efficient multi-scale adapter for synthetic-speech detection</a>, and the DFKI-SLT system for the ESDD 2026 challenge.</span>
  </li>
  <li>
    <span class="news-date">2025-12</span>
    <span class="news-body"><span class="news-tag tag-talk">talk</span>Invited talk at <b>Alexandria University</b> on Speech AI and Arabic pronunciation. <a href="https://www.youtube.com/watch?v=82v05REnNvo">Video on YouTube</a>.</span>
  </li>
  <li>
    <span class="news-date">2025-10-25</span>
    <span class="news-body"><span class="news-tag tag-code">code</span>Released code for <a href="https://github.com/Yaselley/TwoViews_OneTruth"><b>Two Views, One Truth</b></a>.</span>
  </li>
  <li>
    <span class="news-date">2025-10-22</span>
    <span class="news-body"><span class="news-tag tag-talk">talk</span>Invited talk at <a href="https://www.realitydefender.com/">Reality Defender</a> on <a href="https://docs.google.com/presentation/d/1jH2z-_WUoXEDicsIszbYa81h1nIOMqZwfndiom6lnOo/edit">Generalizable Audio Deepfake Detection</a>.</span>
  </li>
  <li>
    <span class="news-date">2025-10-15</span>
    <span class="news-body"><span class="news-tag tag-paper">paper</span>Presented <a href="https://arxiv.org/pdf/2507.20417"><b>Two Views, One Truth</b></a> at WASPAA 2025 (Tahoe City, USA).</span>
  </li>
  <li>
    <span class="news-date">2025-09</span>
    <span class="news-body"><span class="news-tag tag-grant">grant</span>WASPAA 2025 Travel Grant ($1,000).</span>
  </li>
  <li>
    <span class="news-date">2025-08</span>
    <span class="news-body"><span class="news-tag tag-org">organize</span>Co-organized the <a href="https://www.linkedin.com/feed/update/urn:li:activity:7364633218228142083/">ArabicSpeech Meetup</a> at Interspeech 2025.</span>
  </li>
  <li>
    <span class="news-date">2025-06</span>
    <span class="news-body"><span class="news-tag tag-org">organize</span>Founded and led the <a href="https://huggingface.co/IqraEval"><b>Iqra'Eval Shared Task</b></a> at ArabicNLP 2025.</span>
  </li>
  <li>
    <span class="news-date">2025-05</span>
    <span class="news-body"><span class="news-tag tag-paper">paper</span><a href="https://arxiv.org/pdf/2505.13930"><b>BiCrossMamba-ST</b></a>, among the first successful applications of Mamba state-space models to speech anti-spoofing.</span>
  </li>
  <li>
    <span class="news-date">2025-03</span>
    <span class="news-body"><span class="news-tag tag-visit">role</span>Joined <b><a href="https://gretchen-ai.com/">Gretchen AI</a></b> as Research &amp; Engineering Lead (part-time), co-leading R&amp;D for generative-media detection.</span>
  </li>
  <li>
    <span class="news-date">2025-02</span>
    <span class="news-body"><span class="news-tag tag-paper">paper</span><a href="https://arxiv.org/pdf/2502.00894"><b>MorphBPE</b></a>, the morpho-aware tokenizer used in <a href="https://arxiv.org/pdf/2501.13944">Fanar</a>, is out.</span>
  </li>
  <li>
    <span class="news-date">2025-01</span>
    <span class="news-body"><span class="news-tag tag-paper">paper</span><b>Layer-wise Analysis of SSL Models for Audio Deepfake Detection</b> accepted at Findings of NAACL 2025.</span>
  </li>
  <li>
    <span class="news-date">2024-12</span>
    <span class="news-body"><span class="news-tag tag-visit">visit</span>Invited researcher at the <a href="https://sdaia-event.webflow.io/">SDAIA Winter School</a>, leading a team of 15 researchers to build <b>QuranMB</b>, the first expert-annotated dataset for Quranic mispronunciation.</span>
  </li>
</ul>

<div class="section-title">📜 Selected Publications</div>

<p style="font-size:0.9em; color:#64748b; margin-top:-0.2em;">
Full list: <a href="{{ '/publications/' | relative_url }}">publications page</a> and <a href="https://scholar.google.com/citations?user=KATQHwgAAAAJ">Google Scholar</a>
</p>

<ul class="pub-list">
  <li>
    <span class="pub-venue">arXiv 2026</span>
    <span class="pub-title"><a href="https://arxiv.org/abs/2604.08450">DeepFense: A Unified, Modular, and Extensible Framework for Robust Deepfake Audio Detection</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, A. Das, Y. Xiao, X. Wang, F. Kallel, E. E. Erdogan, N. T. Vu, T. Polzehl, S. Möller</span>
  </li>
  <li>
    <span class="pub-venue">arXiv 2026</span>
    <span class="pub-title"><a href="https://arxiv.org/abs/2603.29087">IQRA 2026: Interspeech Challenge on Automatic Pronunciation Assessment for MSA</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, A. Meghanani, M. Shahin, O. Ibrahim, S. A. Chowdhury, et al.</span>
  </li>
  <li>
    <span class="pub-venue">ICASSP 2026</span>
    <span class="pub-title"><a href="https://arxiv.org/abs/2510.24852">A Parameter-Efficient Multi-Scale Convolutional Adapter for Synthetic Speech Detection</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, F. Ritter-Gutiérrez, A. Das, T. Polzehl, S. Möller</span>
  </li>
  <li>
    <span class="pub-venue">ICASSP 2026</span>
    <span class="pub-title">The DFKI-SLT System for ESDD 2026: BiCrossMamba-ST with Attentive SSL Fusion</span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, A. Das, E. E. Erdogan, F. Kallel, T. Polzehl, S. Möller</span>
  </li>
  <li>
    <span class="pub-venue">WASPAA 2025</span>
    <span class="pub-title"><a href="https://arxiv.org/pdf/2507.20417">Two Views, One Truth: Spectral and Self-Supervised Features Fusion for Robust Speech Deepfake Detection</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, A. Das, E. E. Erdogan, F. Ritter-Gutiérrez, T. Polzehl, S. Möller</span>
  </li>
  <li>
    <span class="pub-venue">Interspeech 2025</span>
    <span class="pub-title"><a href="https://arxiv.org/pdf/2505.13930">BiCrossMamba-ST: Speech Deepfake Detection with Bidirectional Mamba Spectro-Temporal Cross-Attention</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, T. Polzehl, S. Möller</span>
  </li>
  <li>
    <span class="pub-venue">NAACL Findings 2025</span>
    <span class="pub-title"><a href="https://arxiv.org/pdf/2502.03559">Comprehensive Layer-wise Analysis of SSL Models for Audio Deepfake Detection</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, Y. Samih, S. Maharjan, T. Polzehl, S. Möller</span>
  </li>
  <li>
    <span class="pub-venue">arXiv 2025</span>
    <span class="pub-title"><a href="https://arxiv.org/pdf/2501.13944">Fanar: An Arabic-Centric Multimodal Generative AI Platform</a></span><br>
    <span class="pub-authors">Fanar Team (incl. <span class="me">Y. El Kheir</span>)</span>
  </li>
  <li>
    <span class="pub-venue">arXiv 2025</span>
    <span class="pub-title"><a href="https://arxiv.org/pdf/2502.00894">MorphBPE: A Morpho-Aware Tokenizer Bridging Linguistic Complexity for Efficient LLM Training Across Morphologies</a></span><br>
    <span class="pub-authors">E. Asgari, <span class="me">Y. El Kheir</span>, M. A. S. Javaheri</span>
  </li>
  <li>
    <span class="pub-venue">ACL 2024</span>
    <span class="pub-title"><a href="https://arxiv.org/pdf/2408.02430">Beyond Orthography: Automatic Recovery of Short Vowels and Dialectal Sounds in Arabic</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, H. Mubarak, A. Ali, S. A. Chowdhury</span>
  </li>
  <li>
    <span class="pub-venue">ICASSP 2024</span>
    <span class="pub-title"><a href="https://arxiv.org/pdf/2309.07719">L1-aware Multilingual Mispronunciation Detection Framework</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, S. A. Chowdhury, A. Ali</span>
  </li>
  <li>
    <span class="pub-venue">Interspeech 2023</span>
    <span class="pub-title"><a href="https://arxiv.org/pdf/2305.07445">QVoice: Arabic Speech Pronunciation Learning Application</a></span><br>
    <span class="pub-authors"><span class="me">Y. El Kheir</span>, F. Khnaisser, S. A. Chowdhury, H. Mubarak, S. Afzal, A. Ali</span>
  </li>
</ul>

<div class="section-title">🎤 Invited Talks &amp; Selected Visits</div>

<ul class="talk-list">
  <li>
    <span class="talk-date">2026-05</span>
    <span class="talk-body"><b><a href="https://hackai.ma">HackAI Morocco 2026</a></b>, Speech ML Mentor (2nd year) and panelist on the PhD Students Panel.</span>
  </li>
  <li>
    <span class="talk-date">2025-12</span>
    <span class="talk-body"><b>Alexandria University</b>, invited talk on Speech AI and Arabic pronunciation. <a href="https://www.youtube.com/watch?v=82v05REnNvo">Video on YouTube</a>.</span>
  </li>
  <li>
    <span class="talk-date">2025-10</span>
    <span class="talk-body"><b><a href="https://www.realitydefender.com/">Reality Defender</a></b>, invited talk on <a href="https://docs.google.com/presentation/d/1jH2z-_WUoXEDicsIszbYa81h1nIOMqZwfndiom6lnOo/edit">Generalizable Audio Deepfake Detection</a>.</span>
  </li>
  <li>
    <span class="talk-date">2025-10</span>
    <span class="talk-body"><b>WASPAA 2025</b>, Tahoe City, paper presentation on Two Views, One Truth.</span>
  </li>
  <li>
    <span class="talk-date">2025-08</span>
    <span class="talk-body"><b>Interspeech 2025</b>, Rotterdam, co-organized the ArabicSpeech Meetup.</span>
  </li>
  <li>
    <span class="talk-date">2025-05</span>
    <span class="talk-body"><b><a href="https://hackai.ma">HackAI Morocco 2025</a></b>, Speech ML Mentor on ASR and forced alignment for low-resource dialects.</span>
  </li>
  <li>
    <span class="talk-date">2024-12</span>
    <span class="talk-body"><b><a href="https://sdaia-event.webflow.io/">SDAIA Winter School</a></b>, Riyadh, invited researcher, led the QuranMB project team.</span>
  </li>
  <li>
    <span class="talk-date">2024</span>
    <span class="talk-body"><b>SDAIA Summer School</b>, invited researcher in the speech and language program.</span>
  </li>
</ul>

<div class="section-title">💼 Experience</div>

<ul class="exp-list">
  <li>
    <div class="exp-logo"><img src="{{ '/images/projects/dfki.png' | relative_url }}" alt="DFKI"></div>
    <div class="exp-body">
      <span class="exp-role">PhD Researcher</span>, <span class="exp-where">DFKI &amp; TU Berlin</span><br>
      <span class="exp-when">2024 to present</span><br>
      <small>Speech foundation models, SSL interpretability, Mamba for audio, multimodal robustness. DeepFense framework, News-Polygraph contributor.</small>
    </div>
  </li>
  <li>
    <div class="exp-logo"><img src="{{ '/images/projects/gretchen.svg' | relative_url }}" alt="Gretchen AI"></div>
    <div class="exp-body">
      <span class="exp-role">Research &amp; Engineering Lead (part-time)</span>, <span class="exp-where">Gretchen AI, Berlin</span><br>
      <span class="exp-when">Mar 2025 to present</span><br>
      <small>Co-leading R&amp;D for generative-media detection. #1 on Deepfake-Eval 2024 benchmark for image deepfake detection.</small>
    </div>
  </li>
  <li>
    <div class="exp-logo"><img src="{{ '/images/projects/qcri.svg' | relative_url }}" alt="QCRI"></div>
    <div class="exp-body">
      <span class="exp-role">Research Associate</span>, <span class="exp-where">Qatar Computing Research Institute (QCRI)</span><br>
      <span class="exp-when">2022 to 2024</span><br>
      <small>Fanar LLM (MorphBPE tokenizer, large-scale training pipelines) and QVoice (Arabic pronunciation learning). 6+ papers in 2 years.</small>
    </div>
  </li>
</ul>

<p style="font-size:0.9em; color:#475569;">
<b>Education:</b> PhD, TU Berlin / DFKI (2024, exp. 2027). MSc Machine Learning, KTH Royal Institute of Technology (2021, 2022). MSc Data Science, EURECOM &amp; Télécom Paris (2020, 2021). Diplôme d'Ingénieur, Télécom Paris (2019, 2022, top 5%).
</p>

<div class="section-title">🏅 Awards &amp; Grants</div>

<ul class="award-list">
  <li><span class="award-year">2025</span> WASPAA 2025 Travel Grant ($1,000)</li>
  <li><span class="award-year">2025</span> ArabicNLP 2025 Grant ($500), for leadership of the Iqra'Eval Shared Task</li>
  <li><span class="award-year">2022</span> Télécom Paris Scholarship, tuition waiver plus stipend for KTH Sweden</li>
  <li><span class="award-year">2019</span> FIRSI Excellence Scholarship (€9,000/year)</li>
  <li><span class="award-year">2018</span> Prépa FIRSI Scholarship</li>
</ul>

<div class="section-title">🤝 Mentorship &amp; Service</div>

I'm currently supervising <b>Enes Erdogan</b> and <b>Feidi Kallel</b> (MSc students at TU Berlin), and have mentored teams at the <b>SDAIA Winter School</b>, <b>SDAIA Summer School</b>, <b>HackAI Morocco</b> (2025 and 2026), and through the <b>Iqra'Eval</b> initiative.

If you're a Master's student in Germany or the EU interested in speech and audio ML, foundation models, ASR/TTS, audio LLMs, deepfake detection, or Arabic / low-resource speech, feel free to reach out. See the <a href="{{ '/talks/' | relative_url }}">Supervision</a> page for details.

**Program Committee & Reviewing:** ACL 2024, ACL 2025, EMNLP 2024, Interspeech 2025, ICASSP 2025, EACL 2025, COLING 2024/25, ArabicNLP 2025, SLaTE 2025. Full list on the <a href="{{ '/teaching/' | relative_url }}">Services</a> page.

<div class="section-title">📬 Contact</div>

<p style="font-size:0.95em;">
📧 <a href="mailto:yassine.el_kheir@dfki.de">yassine.el_kheir@dfki.de</a> &nbsp;&middot;&nbsp;
📧 <a href="mailto:elkheiryassine0@gmail.com">elkheiryassine0@gmail.com</a><br>
🎓 <a href="https://scholar.google.com/citations?user=KATQHwgAAAAJ">Google Scholar</a> &nbsp;&middot;&nbsp;
💻 <a href="https://github.com/Yaselley">GitHub</a> &nbsp;&middot;&nbsp;
🔗 <a href="https://www.linkedin.com/in/yassine-elkheir-169b97191/">LinkedIn</a>
</p>
