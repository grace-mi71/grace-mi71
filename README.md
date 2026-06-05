%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% GANGMIN LEE — Resume (Boltach Anton layout adapted)
% Based on "Boltach Anton's Résumé" Overleaf community article (CC BY 4.0)
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\documentclass[paper=a4,fontsize=11pt]{scrartcl} % KOMA-article class

\usepackage[english]{babel}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}

\usepackage[protrusion=true,expansion=true]{microtype}
\usepackage{amsmath,amsfonts,amsthm}
\usepackage{graphicx}
\usepackage[svgnames]{xcolor}
\usepackage{geometry}
\usepackage{url}
\usepackage{hyperref}
\usepackage{sectsty}
\usepackage{enumitem}

% ---------- Page ----------
\geometry{left=1.6cm,right=1.6cm,top=1.5cm,bottom=1.6cm}
\textheight=700px % template-style compactness
\frenchspacing
\pagestyle{empty}

% ---------- Links ----------
\hypersetup{
  colorlinks=true,
  urlcolor=MidnightBlue,
  linkcolor=MidnightBlue
}

% ---------- Section style ----------
\sectionfont{%
  \usefont{OT1}{phv}{b}{n}%
  \sectionrule{0pt}{0pt}{-5pt}{3pt}
}

% ---------- Macros (from template) ----------
\newlength{\spacebox}
\settowidth{\spacebox}{8888888888} % alignment box

\newcommand{\sepspace}{\vspace*{1em}}

\newcommand{\MyName}[1]{%
  \Huge \usefont{OT1}{phv}{b}{n} \hfill #1
  \par \normalsize \normalfont
}

\newcommand{\MySlogan}[1]{%
  \large \usefont{OT1}{phv}{m}{n}\hfill \textit{#1}
  \par \normalsize \normalfont
}

\newcommand{\NewPart}[1]{\section*{\uppercase{#1}}}

\newcommand{\PersonalEntry}[2]{%
  \noindent\hangindent=2em\hangafter=0
  \parbox{\spacebox}{\textit{#1}}%
  \hspace{1.5em} #2 \par
}

\newcommand{\SkillsEntry}[2]{%
  \noindent\hangindent=2em\hangafter=0
  \parbox{\spacebox}{\textit{#1}}%
  \hspace{1.5em} #2 \par
}

\newcommand{\EducationEntry}[4]{%
  \noindent \textbf{#1} \hfill
  \colorbox{Black}{%
    \parbox{6.8em}{\hfill\color{White}#2}} \par
  \noindent \textit{#3} \par
  \noindent\hangindent=2em\hangafter=0 \small #4
  \normalsize \par
}

\newcommand{\WorkEntry}[4]{%
  \noindent \textbf{#1} \hfill
  \colorbox{Black}{\color{White}#2} \par
  \noindent \textit{#3} \par
  \noindent\hangindent=2em\hangafter=0 \small #4
  \normalsize \par
}

% ---------- Bullet tuning ----------
\setlist[itemize]{leftmargin=1.4em, itemsep=0.25em, topsep=0.2em}

% ---------- Document ----------
\begin{document}

% ===== Header (photo + name) =====
% Upload "portrait.jpg" to your project files
\includegraphics[width=0.30\textwidth]{portrait.jpg}
\MyName{GANGMIN LEE}
\MySlogan{Computer Vision for Structured Visual and Geospatial Signals}

\sepspace

% ===== Personal details =====
\NewPart{Personal details}

\PersonalEntry{Location}{Suwon \& Seoul, South Korea}
\PersonalEntry{Email}{\href{mailto:jerry3708@ajou.ac.kr}{jerry3708@ajou.ac.kr}}
\PersonalEntry{Birth}{2002.07.01}
\PersonalEntry{Phone}{+82 10-2303-2064}
\PersonalEntry{University}{Ajou University}
\PersonalEntry{Major}{Digital-Media \& Software-Engineering (Double Major)}
\PersonalEntry{Military}{Completed \emph{(2023.06 $\sim$ 2024.12)}}
\PersonalEntry{GPA}{3.73 / 4.5}

\sepspace

% ===== Profile & Summary =====
\NewPart{Profile \& Summary}

Cross-disciplinary undergraduate student in \textbf{Digital Media and Software Engineering}, with research experience in \textbf{computer vision, diffusion-based anomaly detection, temporal signal modeling, and spatial representation learning}.\
My work has focused on modeling structured visual signals, including surface defects, human motion sequences, and patch-wise geometric deformation.\
I am currently expanding my research direction toward \textbf{remote sensing AI and geospatial computer vision}, with particular interest in satellite image understanding, anomaly and change detection, disaster monitoring, and SAR/optical data analysis.\
I aim to develop reliable learning-based systems that can interpret large-scale Earth observation data for environmental, urban, and safety-critical applications.
\sepspace

% ===== Skills =====
\NewPart{Skills}

\SkillsEntry{Languages}{Python}
\SkillsEntry{Data/Backend}{FastAPI}
\SkillsEntry{Frontend/Tools}{HTML/CSS/JS (basic), Git/GitHub, LaTeX/Overleaf, Illustrator/Lightroom}

\sepspace

% ===== Education & Research =====
\NewPart{Education \& Research}

\EducationEntry
{Ajou University --- B.S. (Double Major), Digital Media \& Software Engineering}
{2021 -- Ongoing}
{Suwon, KR}
{
\begin{itemize}
  \item \textbf{MainCourse}: Computer Graphics, Image-Processing, Computer Structure, Linear Algebra, Creative-Media Programming, Algorithms
  \item Undergraduate Intern in \textbf{Ajou University CG Lab}; 
  \emph{(2022.10 $\sim$ 2023.04 / 2026.03 $\sim$ current)}
  \item Selected for the \textbf{KENTECH Winter Internship Program}; conducted research on \textbf{diffusion-based anomaly detection} for structural crack analysis at \textbf{ENVI Lab}. \emph{(2025.12 $\sim$ 2026.01)}
\end{itemize}
}

\sepspace

% ===== Artistic & Extracurricular =====
\NewPart{Artistic \& Extracurricular}

\WorkEntry
{A.SA. Central Photography Club --- Executive Member, Ajou Univ.}
{2022.02 -- Current}
{Seoul/Suwon, KR}
{
\begin{itemize}
\item Served consecutive terms as \textbf{Treasurer}, \textbf{Research Team Member}, and \textbf{Vice President}, contributing to both organizational management and creative direction.

  \item Planned and exhibited series \emph{“The Texture of Emotions Shaped by the Gaze”} (Itaewon, 2022.11).
  \item Planned and exhibited series \emph{“Reality and Ideal”} (Seongsu-dong, 2025.11).
  \item Led exhibition planning by exploring and selecting spaces aligned with thematic concepts; designed \textbf{olfactory elements (custom perfume)} and \textbf{interactive programs} to enhance audience experience.

\end{itemize}
}

\sepspace

% ===== Projects =====
\NewPart{Projects}

\WorkEntry
{Preset-Based Patchwise Decomposition for 3D Avatar Expression Transfer}
{2026.03 -- 2026.06}
{Computer Graphics Lab, Ajou University}
{
\begin{itemize}
  \item Proposed a patch-based expression transfer method that decomposes built-in avatar expression presets into semantic facial regions, including the mouth, eyes, brows, and jaw.
  \item Constructed localized deformation bases and reconstructed target expressions using nonnegative least-squares combinations of patch-wise components.
  \item Designed synthetic ground-truth experiments using ARKit 52 blendshapes and compared the proposed method against preset-only selection and global preset mixing.
  \item Published and presented at \textbf{Korea Computer Graphics Society Conference 2026 (KCGS 2026)}.
\end{itemize}
}
\sepspace

\WorkEntry
{Unity-based Drone Reinforcement Learning Environment}
{2026.03 -- 2026.06}
{Paran semester, Ajou University}
{
\begin{itemize}
  \item Led the \textbf{DronePhysics} module in a Unity/ML-Agents project for autonomous drone learning.
  \item Implemented a \textbf{6-DOF rigidbody-based flight controller} with PID-based altitude, roll, pitch, and yaw stabilization.
  \item Added reset logic, velocity limits, and zero-input damping to improve simulation stability and training reliability.
  \item Built test scenes and PlayMode tests to validate yaw stability after reset, heading response to yaw commands, and horizontal drift damping.
\end{itemize}
}
\sepspace

\WorkEntry
{Diffusion-based Unsupervised Crack Anomaly Detection}
{2025.12 – 2026.04}
{ENVI Lab, KENTECH Winter Internship}
{
\begin{itemize}
  \item Analyzed structural false positives in diffusion-based reconstruction anomaly detection (normal-only training).
  \item Designed Linear Structure Weighted Loss with pixel-wise weighting using Structure Tensor and Frangi-Filter priors.
  \item Proposed Diffusion-based Crack Saliency Verification to reinterpret residuals via structural prior and reconstruction consistency.
  \item Published and presented at \textbf{JCCI Conference} (Poster) on diffusion-based crack anomaly detection. 
\end{itemize}
}
\sepspace

\WorkEntry
{SIGN UP! --- Real-time sign language learning system}
{2025.09 -- 2025.12}
{Google-Ajou Univ AI Capstone Design Competition \href{https://github.com/GooChiSo}{(GitHub)}}
{
\begin{itemize}
  \item Designed a human--computer interaction system that enables users to learn sign language through \textbf{motion-based, real-time feedback} rather than passive video imitation.
  \item Built a \textbf{temporal data pre-processing pipeline} for hand keypoint sequences, addressing missing frames, inconsistent detection, and variable-length inputs.
  \item Awarded the \textbf{Excellence Award} at the Google--Ajou University AI Convergence Capstone Design Competition (\textbf{5th out of 64 teams}).

\end{itemize}
}

\sepspace

% ===== Research Motivation =====
\NewPart{Research motivation}

My previous research has centered on learning-based interpretation of structured visual signals. In diffusion-based anomaly detection, I studied how reconstruction consistency and structural priors can be used to identify abnormal patterns in surface imagery. In temporal motion modeling, I developed a real-time sign language learning system based on hand keypoint sequences, which required robust preprocessing of noisy and variable-length visual data. These experiences led me to become interested in broader problems where visual signals are not only images, but spatially and temporally structured observations of the real world.

\sepspace

I am now interested in extending these principles to \textbf{remote sensing and satellite-based Earth observation}. Satellite imagery provides large-scale, multi-temporal, and multi-sensor observations, making it a meaningful domain for studying anomaly detection, change detection, disaster monitoring, and environmental interpretation. In particular, I hope to explore how computer vision and deep learning methods can be adapted to geospatial data while considering sensor-specific characteristics, spatial consistency, and real-world reliability.

\sepspace

In the long term, I aim to contribute to \textbf{remote sensing AI systems} that connect computational models with practical decision-making, such as disaster assessment, urban monitoring, infrastructure analysis, and environmental safety inspection.

\sepspace

% ===== Interests =====
\NewPart{Interests}

Remote Sensing AI; Geospatial Computer Vision; Satellite Image Analysis; Anomaly Detection; Change Detection; SAR/Optical Data Fusion; Disaster Monitoring; Urban and Infrastructure Monitoring

\sepspace

\noindent\textbf{Current focus}: Expanding my background in \textbf{diffusion-based anomaly detection, temporal modeling, and structure-aware visual representation} toward \textbf{satellite image understanding and remote sensing applications}, especially anomaly/change detection and disaster or infrastructure monitoring using multi-sensor Earth observation data.

\sepspace

% ===== Awards & Presentations =====
\NewPart{Awards \& presentations}

\begin{itemize}
  \item Google--Ajou University Capstone Design --- \textbf{Excellence Award (ranked 5th out of 64 teams)}
  \item Ajou University SW-Centered University “Mogakso” Program --- \textbf{Winner (ranked 1st out of 25 teams)}
  \item \textbf{JCCI 2026 Conference} --- Poster Presentation, \emph{"Unsupervised Crack Detection via Diffusion-based Saliency Verification"}
\item \textbf{KCGS 2026 Conference} --- Oral/Poster Presentation,
\emph{“Preset-Based Patchwise Decomposition of Facial Deformation Bases for 3D Avatar Expression Transfer.”}
\end{itemize}

\end{document}
