<h1 align="left">Hi, I'm Hatem Saadallah 👋</h1>
<h3 align="left">Machine Learning Engineer · Senior Software Engineer</h3>

<p align="left">
  Building production ML systems at the intersection of computer vision, deep learning, and scalable backend engineering. I care about
  models that <em>actually contribute causally</em> at inference, not just on a leaderboard — and about the engineering rigour to ship them.
</p>

<p align="left">
  📍&nbsp;&nbsp;Currently &nbsp;·&nbsp; MSc in Artificial Intelligence · Bocconi University<br/>
  ✉️&nbsp;&nbsp;<a href="mailto:saadallah.r.hatem@gmail.com">saadallah.r.hatem@gmail.com</a><br/>
</p>

---

### 🚀 Featured projects

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
  <a href="https://www.tensorflow.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/tensorflow-colored.svg" width="36" height="36" alt="TensorFlow" /></a>
  <a href="https://scikit-learn.org/" target="_blank"><img src="https://www.vectorlogo.zone/logos/scikit-learn/scikit-learn-icon.svg" width="36" height="36" alt="scikit-learn" /></a>
  <a href="https://numpy.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/numpy-colored.svg" width="36" height="36" alt="NumPy" /></a>
  <a href="https://pandas.pydata.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/pandas-colored.svg" width="36" height="36" alt="Pandas" /></a>
  <a href="https://huggingface.co/" target="_blank"><img src="https://huggingface.co/front/assets/huggingface_logo-noborder.svg" width="36" height="36" alt="Hugging Face" /></a>
  <a href="https://opencv.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/opencv-colored.svg" width="36" height="36" alt="OpenCV" /></a>
  <a href="https://onnx.ai/" target="_blank"><img src="https://www.vectorlogo.zone/logos/onnxai/onnxai-icon.svg" width="36" height="36" alt="ONNX" /></a>
  <a href="https://jupyter.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/jupyter-colored.svg" width="36" height="36" alt="Jupyter" /></a>
</p>

**Languages**

<p align="left">
  <a href="https://www.python.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/python-colored.svg" width="36" height="36" alt="Python" /></a>
  <a href="https://www.typescriptlang.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/typescript-colored.svg" width="36" height="36" alt="TypeScript" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/javascript-colored.svg" width="36" height="36" alt="JavaScript" /></a>
  <a href="https://docs.microsoft.com/en-us/cpp/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/cplusplus-colored.svg" width="36" height="36" alt="C++" /></a>
  <a href="https://www.oracle.com/java/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/java-colored.svg" width="36" height="36" alt="Java" /></a>
  <a href="https://docs.microsoft.com/en-us/cpp/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/c-colored.svg" width="36" height="36" alt="C" /></a>
  <a href="https://www.php.net/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/php-colored.svg" width="36" height="36" alt="PHP" /></a>
</p>

**Backend, Data & Cloud**

<p align="left">
  <a href="https://nodejs.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/nodejs-colored.svg" width="36" height="36" alt="Node.js" /></a>
  <a href="https://expressjs.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/express-colored.svg" width="36" height="36" alt="Express" /></a>
  <a href="https://docs.nestjs.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/nestjs-colored.svg" width="36" height="36" alt="NestJS" /></a>
  <a href="https://www.djangoproject.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/django-colored.svg" width="36" height="36" alt="Django" /></a>
  <a href="https://flask.palletsprojects.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/flask-colored.svg" width="36" height="36" alt="Flask" /></a>
  <a href="https://graphql.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/graphql-colored.svg" width="36" height="36" alt="GraphQL" /></a>
  <a href="https://www.postgresql.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/postgresql-colored.svg" width="36" height="36" alt="PostgreSQL" /></a>
  <a href="https://www.mongodb.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/mongodb-colored.svg" width="36" height="36" alt="MongoDB" /></a>
  <a href="https://redis.io/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/redis-colored.svg" width="36" height="36" alt="Redis" /></a>
  <a href="https://www.docker.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/docker-colored.svg" width="36" height="36" alt="Docker" /></a>
  <a href="https://aws.amazon.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/aws-colored_1.svg" width="36" height="36" alt="AWS" /></a>
  <a href="https://firebase.google.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/firebase-colored.svg" width="36" height="36" alt="Firebase" /></a>
</p>

**Frontend**

<p align="left">
  <a href="https://reactjs.org/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/react-colored.svg" width="36" height="36" alt="React" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Glossary/HTML5" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/html5-colored.svg" width="36" height="36" alt="HTML5" /></a>
  <a href="https://www.w3.org/TR/CSS/#css" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/css3-colored.svg" width="36" height="36" alt="CSS3" /></a>
  <a href="https://tailwindcss.com/" target="_blank"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/tailwindcss-colored.svg" width="36" height="36" alt="Tailwind CSS" /></a>
</p>

---

### 🎯 What I'm working on

- 🔬 **Computer vision research** — transformer detectors, small-object detection, attention-based refinement (see featured project above).
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
  <a href="mailto:saadallah.r.hatem@gmail.com"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/gmail.svg" width="32" height="32" alt="Gmail" /></a>
</p>

<sub>Open to collaborations on applied ML, computer vision, and ML systems work. Drop me an email.</sub>
