---
permalink: /
title: "Yassine El Kheir"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a PhD researcher at the [German Research Center for AI (DFKI)](https://www.dfki.de/en/web) and [TU Berlin](https://www.tu.berlin/en/), advised by [Sebastian Möller](https://scholar.google.de/citations?user=BC_qcg0AAAAJ) and [Tim Polzehl](https://scholar.google.de/citations?user=tImnUh0AAAAJ). I build speech and audio systems that have to hold up outside a single benchmark: self-supervised representations, small detectors, and speech LLMs that can say why a voice is synthetic. I expect to defend in **April 2027**.

I am looking for research and applied scientist roles from **November 2026**. Write to [elkheiryassine0@gmail.com](mailto:elkheiryassine0@gmail.com). A two-page CV is [here]({{ '/files/Yassine_ElKheir_CV.pdf' | relative_url }}).

## How the work connects

Arabic speech came first. At [QCRI](https://www.hbku.edu.qa/en/qcri) I built pronunciation and recognition systems, including [QVoice](https://arxiv.org/abs/2305.07445), and contributed to [Fanar](https://arxiv.org/abs/2501.13944), Qatar's Arabic-centric multimodal model, including the [MorphBPE](https://arxiv.org/abs/2502.00894) tokenizer.

That turned into a question about representations. A [layer-wise study](https://arxiv.org/abs/2502.03559) of Wav2Vec 2.0, WavLM, and HuBERT showed that early layers carry the deepfake signal, which makes inference about three times faster. [BiCrossMamba-ST](https://www.isca-archive.org/interspeech_2025/elkheir25_interspeech.html) then applied a Mamba model to the same problem, with 28% fewer parameters than a Transformer baseline. The DFKI-SLT system built on it placed [1st of 97 teams](https://sites.google.com/view/esdd-challenge) on Track 2 of the ESDD 2026 challenge at ICASSP, and 2nd on Track 1 ([results](https://arxiv.org/abs/2603.04865)).

The next step is a model that can explain the decision. From December 2025 to April 2026 I visited [NII](https://www.nii.ac.jp/en/) in Tokyo, working with Xin Wang and Junichi Yamagishi on speech LLMs that ground a detection in text. The paper is [Textual Acoustic Grounding](https://arxiv.org/abs/2608.30622), under review at IEEE SLT 2026. Models from that work are on [Hugging Face](https://huggingface.co/01Yassine/AudioLLM-Deepfake-Detection).

The version other people can run is [DeepFense](https://deepfense.github.io/): an open, YAML-driven detection framework with 455+ pretrained models, which I presented at Interspeech 2026. The same line ships at [Gretchen AI](https://gretchen-ai.com/), whose detector ranked first on Deepfake-Eval 2024, and in production speech systems at [CAMB.AI](https://www.camb.ai/) across 150+ languages.

I lead [Fake-O-Meter](https://fake-o-meter.github.io/) and coordinate it day to day. DFKI runs the consortium. The partners are TU Berlin, Otto von Guericke University Magdeburg, Ernst-Abbe-Hochschule Jena, Deutsche Welle, and dpa. The project builds a multimodal assistant for image, audio, and video deepfakes: detection, explanations grounded in professional fact-checks, a dialogue assistant, and prebunking around elections. Fact-checkers stay in the loop. It is funded by the German Federal Ministry of Research, Technology and Space, from May 2026 to February 2029. [Project site](https://fake-o-meter.github.io/). [DFKI page](https://www.dfki.de/web/forschung/projekte-publikationen/projekt/fake-o-meter).

I also lead **VERIDIC**, and a [Software Campus](https://www.softwarecampus.de/) project with Holtzbrinck and Springer Nature: €115k in federal funding, from July 2026, on multimodal deepfake detection and fact-checking, with a team of students and research assistants.

## Recent

- **October 2026.** Invited talk at the [GrokBot Casablanca Meetup](https://luma.com/spacexai-slxi): *MoulSot, the first Darija ASR model*, with Abdeljalil El Majjodi. [MoulSot](https://huggingface.co/blog/abdeljalilELmajjodi/moulsot).
- **September 2026.** [Interspeech 2026](https://www.isca-archive.org/interspeech_2026), Sydney. I presented [DeepFense](https://arxiv.org/abs/2604.08450) and the [IQRA 2026](https://arxiv.org/abs/2603.29087) challenge, and co-authored [Evidence Subspace Projection](https://arxiv.org/abs/2607.11538) with the University of Stuttgart.
- **July 2026.** Co-organized [ArA-DF 2026](https://huggingface.co/spaces/ArabicSpeech/ara-df-2026), the Arabic speech deepfake detection shared task at ArabicNLP, co-located with EMNLP 2026. Sixteen teams, two tracks.
- **July 2026.** I lead a [Software Campus](https://www.softwarecampus.de/) project with Holtzbrinck and Springer Nature (€115k, federal funding) on multimodal deepfake detection and fact-checking, and I lead **VERIDIC**.
- **May 2026.** [Fake-O-Meter](https://fake-o-meter.github.io/) starts. I lead the project and coordinate the partners day to day. [DFKI page](https://www.dfki.de/web/forschung/projekte-publikationen/projekt/fake-o-meter).
- **May 2026.** Speech ML mentor and PhD panelist at [HackAI Morocco](https://hackai.ma).
- **April 2026.** Finished the visiting stay at NII Tokyo. [Paper](https://arxiv.org/abs/2608.30622).

## Talks

GrokBot and Interspeech 2026 are in the list above. Slides, video, and the earlier talks are on the [talks page]({{ '/talks/' | relative_url }}).

- **Alexandria University**, December 2025. Speech AI and Arabic pronunciation. [Video](https://www.youtube.com/watch?v=82v05REnNvo).
- **Reality Defender**, October 2025. Generalizable audio deepfake detection. [Slides](https://docs.google.com/presentation/d/1jH2z-_WUoXEDicsIszbYa81h1nIOMqZwfndiom6lnOo/edit).
- **WASPAA 2025**, Tahoe City. [Two Views, One Truth](https://arxiv.org/abs/2507.20417). [Code](https://github.com/Yaselley/TwoViews_OneTruth).
- **Interspeech 2025**, Rotterdam. [BiCrossMamba-ST](https://www.isca-archive.org/interspeech_2025/elkheir25_interspeech.html), and the [ArabicSpeech meetup](https://www.linkedin.com/posts/yassine-el-kheir-169b97191_interspeech2025-interspeech-arabicspeech-activity-7364633218228142083-IBv-).

## Selected work

- **[DeepFense](https://deepfense.github.io/).** Open framework for audio deepfake detection. [Paper](https://arxiv.org/abs/2604.08450), [code](https://github.com/Yaselley/deepfense-framework), [models](https://huggingface.co/DeepFense).
- **Detectors.** [BiCrossMamba-ST](https://arxiv.org/abs/2505.13930), [layer-wise SSL analysis](https://arxiv.org/abs/2502.03559), [spectral and SSL fusion](https://arxiv.org/abs/2507.20417), [multi-scale adapter](https://arxiv.org/abs/2510.24852). ESDD 2026: [1st and 2nd](https://arxiv.org/abs/2603.04865).
- **Speech LLMs.** [Textual Acoustic Grounding](https://arxiv.org/abs/2608.30622), with Xin Wang and Junichi Yamagishi at NII. [Models](https://huggingface.co/01Yassine/AudioLLM-Deepfake-Detection).
- **Production.** [Gretchen AI](https://gretchen-ai.com/) (first on Deepfake-Eval 2024) and [CAMB.AI](https://www.camb.ai/) (ASR, TTS, and dubbing in 150+ languages).
- **Language.** [MoulSot](https://huggingface.co/blog/abdeljalilELmajjodi/moulsot) with [AtlasIA](https://atlasia.ma/), the [Iqra'Eval](https://huggingface.co/IqraEval) / [IQRA 2026](https://arxiv.org/abs/2603.29087) pronunciation challenge, and [Fanar](https://arxiv.org/abs/2501.13944) / [MorphBPE](https://arxiv.org/abs/2502.00894).
- **Leading.** [Fake-O-Meter](https://fake-o-meter.github.io/) (project lead and day-to-day coordination, May 2026 to February 2029), [Software Campus](https://www.softwarecampus.de/) with Holtzbrinck and Springer Nature, and VERIDIC.

The [projects page]({{ '/projects/' | relative_url }}) has the longer notes.

## Selected papers

Full list on the [publications page]({{ '/publications/' | relative_url }}) and on [Google Scholar](https://scholar.google.com/citations?user=KATQHwgAAAAJ).

- Y. El Kheir et al. [DeepFense: A Unified, Modular Framework for Robust Deepfake Audio Detection](https://arxiv.org/abs/2604.08450). Interspeech 2026.
- Y. El Kheir et al. [IQRA 2026: Interspeech Challenge on Automatic Pronunciation Assessment for MSA](https://arxiv.org/abs/2603.29087). Interspeech 2026.
- Y. Xiao, Y. El Kheir, et al. [Evidence Subspace Projection](https://arxiv.org/abs/2607.11538). Interspeech 2026.
- Y. El Kheir et al. [Textual Acoustic Grounding for Generalizable LLM-Based Deepfake Voice Detection](https://arxiv.org/abs/2608.30622). IEEE SLT 2026, under review.
- Y. El Kheir et al. [A Parameter-Efficient Multi-Scale Adapter for Synthetic Speech Detection](https://arxiv.org/abs/2510.24852). ICASSP 2026.
- Y. El Kheir et al. DFKI-SLT for ESDD 2026: BiCrossMamba-ST with Attentive SSL Fusion. ICASSP 2026. [Results](https://arxiv.org/abs/2603.04865).
- Y. El Kheir, T. Polzehl, S. Möller. [BiCrossMamba-ST](https://www.isca-archive.org/interspeech_2025/elkheir25_interspeech.html). Interspeech 2025.
- Y. El Kheir et al. [Layer-wise Analysis of SSL Models for Audio Deepfake Detection](https://arxiv.org/abs/2502.03559). Findings of NAACL 2025.

## Positions

- **PhD researcher**, DFKI and TU Berlin, 2024 to present. Advisors: Sebastian Möller and Tim Polzehl.
- **Project lead, [Fake-O-Meter](https://fake-o-meter.github.io/)**, May 2026 to February 2029. I lead the project and coordinate the consortium day to day: TU Berlin, OVGU Magdeburg, Ernst-Abbe-Hochschule Jena, Deutsche Welle, and dpa. DFKI is the coordinator. Funded by the BMFTR. [Project site](https://fake-o-meter.github.io/). [DFKI record](https://www.dfki.de/web/forschung/projekte-publikationen/projekt/fake-o-meter).
- **Project lead, Software Campus**, July 2026 to present. I lead a €115k federally funded project with [Holtzbrinck and Springer Nature](https://www.softwarecampus.de/) on multimodal deepfake detection and fact-checking, with a team of students and research assistants.
- **Project lead, VERIDIC.**
- **Visiting researcher**, NII, Tokyo, December 2025 to April 2026. Xin Wang and Junichi Yamagishi.
- **Founding research scientist** (part-time), [Gretchen AI](https://gretchen-ai.com/), Berlin, January 2025 to present.
- **Research consultant**, [CAMB.AI](https://www.camb.ai/), April 2025 to present. Multilingual ASR, TTS, and dubbing.
- **Research associate**, [QCRI](https://www.hbku.edu.qa/en/qcri), Doha, 2022 to 2024. Fanar and QVoice.

**Education.** PhD, Computer Science, TU Berlin / DFKI, 2024 to 2027, defense expected April 2027. MSc, Machine Learning, KTH Royal Institute of Technology, 2022. Diplôme d'Ingénieur, Télécom Paris, 2022, top 5%.

## Collaboration

I work with students and researchers anywhere. Master's theses, research visits, and joint papers are all welcome: speech foundation models, audio deepfake detection, speech LLMs, ASR and TTS, pronunciation, and low-resource speech, including Arabic and Darija.

Current students and how to write are on the [talks and collaboration page]({{ '/talks/#collaboration' | relative_url }}).

## Contact

[elkheiryassine0@gmail.com](mailto:elkheiryassine0@gmail.com) · [yassine.el_kheir@dfki.de](mailto:yassine.el_kheir@dfki.de) · [Google Scholar](https://scholar.google.com/citations?user=KATQHwgAAAAJ) · [GitHub](https://github.com/Yaselley) · [LinkedIn](https://www.linkedin.com/in/yassine-el-kheir-169b97191/) · [CV]({{ '/files/Yassine_ElKheir_CV.pdf' | relative_url }})
