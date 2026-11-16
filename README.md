<h1 align="left">Hi, I'm Hatem Saadallah 👋</h1>
<h3 align="left">Machine Learning Engineer · Software Engineer</h3>

<p align="left">
  Building production ML systems at the intersection of computer vision, LLM agents, and scalable backend engineering.
  I care about models whose gains survive a held-out test and code that other people can run.
</p>

<p align="left">
  🎓&nbsp;&nbsp;MSc Artificial Intelligence student · Bocconi University<br/>
  📍&nbsp;&nbsp;Milan, Italy<br/>
  💼&nbsp;&nbsp;<a href="https://www.linkedin.com/in/hatem-r-sadallah/">LinkedIn</a><br/>
  ✉️&nbsp;&nbsp;<a href="mailto:saadallah.r.hatem@gmail.com">saadallah.r.hatem@gmail.com</a><br/>
</p>

---

### 🚀 Featured projects

<table>
  <tr>
    <td width="55%" valign="top">
      <h4>👁️ <a href="https://github.com/HatemSaadallah/aemon">aemon: a strategy-investigation agent</a></h4>
      <p><sub>LLM Agents · Agentic Fine-tuning · Evaluation</sub></p>
      <p>
        Teaches a <strong>3B open model</strong> (Tiny Aya Global) to investigate a strategy question the way a careful analyst would: frame the decision, state rival explanations, weigh quoted evidence for and against each, look for what would prove the favourite wrong, propose a test, and revise when new evidence arrives. Twelve guarded tools and a stage controller enforce the procedure: a quote that is not word for word in its source is refused, and every run replays step by step.
      </p>
      <p>
        <strong>Result:</strong> <strong>+0.83</strong> blind quality over the best-prompted base model on a frozen test run once (0–3 scale, 95% CI 0.69 to 0.97), and <strong>+0.52</strong> on a second frozen test of 12 unseen companies. The final system finishes <strong>46 of 48</strong> investigations against the base model's 4, in 39 tool calls against 242. Distilled from Command A+: only teacher runs that replayed exactly became training data.
      </p>
      <p>
        <em>AgentTune (LoRA) · AuditKIT · PEFT / TRL · llama.cpp · FastAPI · React · Hugging Face · SLURM</em>
      </p>
      <p>
        <a href="https://github.com/HatemSaadallah/aemon">📦 Repo</a> &nbsp;·&nbsp;
        <a href="https://huggingface.co/spaces/HatemSaadallah/aemon">🖥️ Live demo</a> &nbsp;·&nbsp;
        <a href="https://huggingface.co/two-eyed-ravens/aemon">🤗 Model</a> &nbsp;·&nbsp;
        <a href="https://huggingface.co/datasets/two-eyed-ravens/aemon">🗂️ Dataset</a> &nbsp;·&nbsp;
        <a href="https://huggingface.co/blog/HatemSaadallah/aemon">📝 Article</a> &nbsp;·&nbsp;
        <a href="https://github.com/HatemSaadallah/aemon/blob/main/docs/PAPER.pdf">📄 Paper (PDF)</a>
      </p>
    </td>
    <td width="45%" valign="top">
      <a href="https://github.com/HatemSaadallah/aemon">
        <picture>
          <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/HatemSaadallah/aemon/main/docs/figures/quality-dark.png" />
          <img src="https://raw.githubusercontent.com/HatemSaadallah/aemon/main/docs/figures/quality-light.png" alt="Final test, four companies never seen in training: blind quality 1.48 fine-tuned against 0.65 for the base model" />
        </picture>
      </a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td width="55%" valign="top">
      <h4>🖼️ <a href="https://github.com/HatemSaadallah/feedback-augmented-rtdetr">Feedback-Augmented RT-DETR</a></h4>
      <p><sub>Computer Vision · Real-time Detection · Transformers</sub></p>
      <p>
        A novel <strong>decoder-to-encoder feedback module</strong> for real-time object detection.
        Demonstrates the structural insight that an unconstrained learnable gate can be silently zeroed by the optimizer — and fixes it with a one-line reparameterization (a <em>floor</em> on the gate) and a P2/P3-only level mask.
      </p>
      <p>
        <strong>Result:</strong> +0.99 AP<sub>S</sub> causal contribution on COCO val2017 (33.26 → 34.25), where the v1 baseline of the same mechanism contributed 0.00.
      </p>
      <p>
        <em>PyTorch · CUDA · SLURM · A100 HPC · LaTeX</em>
      </p>
      <p>
        <a href="https://github.com/HatemSaadallah/feedback-augmented-rtdetr">📦 Repo</a> &nbsp;·&nbsp;
        <a href="https://github.com/HatemSaadallah/feedback-augmented-rtdetr/blob/main/report/main.pdf">📄 Report (PDF)</a> &nbsp;·&nbsp;
        <a href="https://github.com/HatemSaadallah/feedback-augmented-rtdetr/blob/main/presentation/feedback_augmented_rtdetr.pdf">🎤 Slides</a>
      </p>
    </td>
    <td width="45%" valign="top">
      <a href="https://github.com/HatemSaadallah/feedback-augmented-rtdetr">
        <img src="https://raw.githubusercontent.com/HatemSaadallah/feedback-augmented-rtdetr/main/report/figures/ablation_bars.png" alt="v2 same-checkpoint ablation: Δ AP_S = +0.99" />
      </a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td width="55%" valign="top">
      <h4>🔤 <a href="https://github.com/HatemSaadallah/irab_project">I'rāb-Guided Arabic Diacritization</a></h4>
      <p><sub>NLP · Multi-task Learning · Low-resource Languages</sub></p>
      <p>
        An <strong>explainable</strong> Arabic NLP system. Unlike pure neural diacritizers, every predicted diacritic comes with a <em>grammatical justification</em> — the i'rāb head doubles as auxiliary training signal (regularizing the encoder) and as an interpretability layer (exposing the model's syntactic reasoning).
      </p>
      <p>
        Three task heads on a shared character-level transformer encoder: <strong>tashkīl</strong> (15-way diacritic classifier), <strong>i'rāb</strong> (11-way grammatical-role classifier), and <strong>error tagger</strong> (BIO over orthographic + grammatical errors). Trained jointly on Tashkeela (~75M words), QAC, I3rab Treebank, and synthetic perturbations with per-sample loss masking.
      </p>
      <p>
        <em>PyTorch Lightning · Transformers · LoRA / QLoRA · SentencePiece · Streamlit · HuggingFace</em>
      </p>
      <p>
        <a href="https://github.com/HatemSaadallah/irab_project">📦 Repo</a>
      </p>
    </td>
    <td width="45%" valign="top">
      <table align="center">
        <tr><td align="center" colspan="2"><sub>Input → Output</sub></td></tr>
        <tr>
          <td align="center" dir="rtl"><h3>ذهب الولدُ</h3></td>
          <td align="center"><sub>(plain text)</sub></td>
        </tr>
        <tr>
          <td align="center"><strong>↓</strong></td>
          <td align="center"></td>
        </tr>
        <tr>
          <td align="center" dir="rtl"><h3>ذَهَبَ الْوَلَدُ</h3></td>
          <td align="center"><sub>+ diacritics</sub></td>
        </tr>
        <tr>
          <td align="center"><strong>↓</strong></td>
          <td align="center"></td>
        </tr>
        <tr>
          <td align="center" dir="rtl"><sub>ذَهَبَ <em>(verb, past)</em><br/>الْوَلَدُ <em>(fāʿil, marfūʿ)</em></sub></td>
          <td align="center"><sub>+ i'rāb</sub></td>
        </tr>
      </table>
    </td>
  </tr>
</table>

---

### 🛠️ Tech stack

**Machine Learning & Deep Learning**

<p align="left">
  <a href="https://pytorch.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/pytorch-colored.svg" width="36" height="36" alt="PyTorch" /></a>
  <a href="https://scikit-learn.org/" target="_blank"><img src="https://www.vectorlogo.zone/logos/scikit-learn/scikit-learn-icon.svg" width="36" height="36" alt="scikit-learn" /></a>
  <a href="https://numpy.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/numpy-colored.svg" width="36" height="36" alt="NumPy" /></a>
  <a href="https://huggingface.co/" target="_blank"><img src="https://huggingface.co/front/assets/huggingface_logo-noborder.svg" width="36" height="36" alt="Hugging Face" /></a>
  <a href="https://onnx.ai/" target="_blank"><img src="https://www.vectorlogo.zone/logos/onnxai/onnxai-icon.svg" width="36" height="36" alt="ONNX" /></a>
</p>

**Languages**

<p align="left">
  <a href="https://www.python.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/python-colored.svg" width="36" height="36" alt="Python" /></a>
  <a href="https://www.typescriptlang.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/typescript-colored.svg" width="36" height="36" alt="TypeScript" /></a>
  <a href="https://docs.microsoft.com/en-us/cpp/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/cplusplus-colored.svg" width="36" height="36" alt="C++" /></a>
</p>

**Backend & Infrastructure**

<p align="left">
  <a href="https://docs.nestjs.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/nestjs-colored.svg" width="36" height="36" alt="NestJS" /></a>
  <a href="https://www.postgresql.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/postgresql-colored.svg" width="36" height="36" alt="PostgreSQL" /></a>
  <a href="https://www.docker.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/docker-colored.svg" width="36" height="36" alt="Docker" /></a>
  <a href="https://aws.amazon.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/aws-colored_1.svg" width="36" height="36" alt="AWS" /></a>
</p>

**Frontend**

<p align="left">
  <a href="https://reactjs.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/react-colored.svg" width="36" height="36" alt="React" /></a>
</p>

---

### 🎯 What I'm working on

- 🕵️ **LLM agents and agentic fine-tuning** — distilling an investigative procedure into small open models, guarded tool use, and blind LLM-judge evaluation (see aemon above).
- 🔬 **Computer vision research** — transformer detectors, small-object detection, attention-based refinement (see RT-DETR above).
- 🛠️ **ML systems engineering** — bridging research code and production: reproducible training pipelines, ablation harnesses, ONNX export, GPU profiling.
- 📚 **Learning** — currently deepening into RL for sequential decision-making and the latest LLM-as-a-tool literature.

---

### 📊 GitHub stats

<p align="left">
  <a href="https://github.com/HatemSaadallah">
    <img src="https://github-readme-stats.vercel.app/api?username=HatemSaadallah&show_icons=true&hide=&count_private=true&title_color=0891b2&text_color=ffffff&icon_color=0891b2&bg_color=1c1917&hide_border=true" alt="HatemSaadallah's GitHub stats" />
  </a>
  <a href="https://github.com/HatemSaadallah">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=HatemSaadallah&stroke=ffffff&background=1c1917&ring=0891b2&fire=0891b2&currStreakNum=ffffff&currStreakLabel=0891b2&sideNums=ffffff&sideLabels=ffffff&dates=ffffff&hide_border=true" alt="GitHub Streak" />
  </a>
</p>
<p align="left">
  <a href="https://github.com/HatemSaadallah">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HatemSaadallah&langs_count=8&layout=compact&title_color=0891b2&text_color=ffffff&icon_color=0891b2&bg_color=1c1917&hide_border=true&locale=en" alt="Top Languages" />
  </a>
</p>

---

### 🤝 Connect

<p align="left">
  <a href="https://github.com/HatemSaadallah" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/github.svg" width="32" height="32" alt="GitHub" /></a>
  <a href="https://www.linkedin.com/in/hatem-r-sadallah/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/linkedin.svg" width="32" height="32" alt="LinkedIn" /></a>
  <a href="mailto:saadallah.r.hatem@gmail.com"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/gmail.svg" width="32" height="32" alt="Gmail" /></a>
</p>

<sub>Open to collaborations on applied ML, computer vision, and ML systems work. Drop me an email.</sub>
