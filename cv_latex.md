%-------------------------
% Resume in LaTeX (ATS-friendly version)
%-------------------------
\documentclass[a4paper,11pt]{article}

\usepackage{ragged2e}
\usepackage[empty]{fullpage}
\usepackage{tabularx}
\usepackage{titlesec}
\usepackage{geometry}
\usepackage{enumitem}
\usepackage[hidelinks]{hyperref}
\usepackage[T1]{fontenc}

\geometry{
    left=1.3cm,
    top=0.4cm,
    right=1.1cm,
    bottom=0.4cm
}

\setlength{\parskip}{0pt}
\setlength{\parindent}{0pt}
\setlength{\tabcolsep}{0in}

% No rule under section titles - simple, plain heading
\titleformat{\section}{
    \raggedright\large\bfseries
}{}{0em}{}
\titlespacing{\section}{0pt}{3pt}{1.5pt}

%-------------------------
% Custom commands
%-------------------------

\newcommand{\resumeSubheading}[4]{
    \item
    \begin{tabularx}{\textwidth}{X r}
        \textbf{#1} & \footnotesize #2 \\
        \footnotesize #3 & \footnotesize #4 \\
    \end{tabularx}
    \vspace{-2mm}
}

\newcommand{\resumeProject}[4]{
    \vspace{0.5mm}\item
    \begin{tabularx}{\textwidth}{X r}
        \textbf{#1} & \footnotesize #3 \\
        \footnotesize #2 & \footnotesize #4 \\
    \end{tabularx}
    \vspace{-1mm}
}

\newcommand{\resumeSubHeadingListStart}{
    \begin{itemize}[leftmargin=*, labelsep=0mm]
}

\newcommand{\resumeSubHeadingListEnd}{
    \end{itemize}\vspace{-2mm}
}

\newcommand{\resumeItemListStart}{
    \begin{itemize}[
        leftmargin=3ex,
        noitemsep,
        itemsep=0mm
    ]
    \small
}

\newcommand{\resumeItemListEnd}{
    \end{itemize}\vspace{-3mm}
}

%-------------------------
% Document
%-------------------------

\begin{document}
\raggedright
\fontfamily{cmr}\selectfont

%----------HEADER----------
{\Large \textbf{Ahmed Arafa}}\\
Backend Engineer\\
Phone: +20 115 335 0972 \quad
Email: \href{mailto:ahmed.arafa.engineer15@gmail.com}{ahmed.arafa.engineer15@gmail.com}\\
LinkedIn: \href{https://www.linkedin.com/in/ahmedarafa1515/}{https://www.linkedin.com/in/ahmedarafa1515/} \quad
GitHub: \href{https://github.com/ahmed151515}{https://github.com/ahmed151515} \quad
Portfolio: \href{https://ahmed151515.github.io/Portfolio/}{https://ahmed151515.github.io/Portfolio/}

\vspace{0mm}

%----------SUMMARY----------
\section{Summary}

\small{
Junior Backend Engineer with a Computer Science background and hands-on experience building REST APIs, relational database workflows, authentication, and background processing in C\# and ASP.NET Core. Comfortable with layered architecture and SOLID principles, and looking to grow into a production backend engineering role.
}

\vspace{0mm}

%----------SKILLS----------
\section{Technical Skills}

\begin{itemize}[leftmargin=0.05in, label={}]
\small{
\item{
    \textbf{Languages:} C\#, Python, SQL
    \\

    \textbf{Concepts:} REST API Design, Authentication/Authorization, Background Jobs, Object-Oriented Programming, SOLID Principles, Layered Architecture, Repository Pattern, Unit of Work, Database Design, Database Management, Asynchronous Programming, Server-Side Pagination, SDLC
    \\

    \textbf{Tools \& Frameworks:} ASP.NET Core, EF Core, PostgreSQL, SQL Server, LINQ, Docker, Git, GitHub, Supabase, Supabase Storage, Postman
    \\

    \textbf{Additional:} TypeScript, Django, Vue 3, Deno
}
}
\end{itemize}

\vspace{0mm}

%----------PROJECTS----------
\section{Projects}

\resumeSubHeadingListStart

%----------EASY COPY----------
\resumeProject
{Easy Copy}
{Temporary cross-device file and note transfer platform}
{Aug 2026}
{Website: \href{https://easy-copy.pages.dev/}{link} \quad GitHub: \href{https://github.com/ahmed151515/easy_copy}{link}}

\resumeItemListStart

\item \textbf{System Design:} Designed a temporary cross-device transfer platform with password-protected sessions, configurable 15, 30, or 60-minute lifetimes, and per-session limits of 100MB storage and 3 notes

\item \textbf{Authentication:} Implemented account-free session authorization using bcrypt-hashed passwords and server-side validation across Deno Edge Functions

\item \textbf{Backend Development:} Built session-scoped file and note workflows using PostgreSQL and Supabase Storage, including signed file transfers, upload progress, and resource limits

\item \textbf{Background Jobs:} Implemented a cron-based cleanup job running every 30 minutes, processing up to 50 expired sessions per run to remove associated files, notes, and session records

\item \textbf{Tech Stack:} Vue 3, TypeScript, Vite, PostgreSQL, Deno Edge Functions

\resumeItemListEnd

%----------SOCIAL MEDIA APP----------
\resumeProject
{Social Media App}
{Community platform with posts, threaded discussions, and user interactions}
{Oct 2025}
{GitHub: \href{https://github.com/ahmed151515/Social_Media_App}{link}}

\resumeItemListStart

\item \textbf{ASP.NET Core MVC:} Built a layered social platform using ASP.NET Core 8.0 MVC, EF Core, and the Repository/Unit of Work patterns to separate business logic from data access

\item \textbf{Asynchronous Programming:} Implemented asynchronous request handling and server-side pagination for posts and comments to avoid loading full result sets into memory

\item \textbf{MVC Architecture:} Structured controllers, views, and models with structured JSON responses where needed, creating a clear boundary between backend logic and frontend clients

\item \textbf{Database Design:} Built database operations with EF Core and SQL Server, including entity relationships, querying, persistence, and LINQ-based data access

\item \textbf{Authentication:} Implemented user authentication and session-based access control for posts and threaded discussions

\item \textbf{Tech Stack:} ASP.NET Core 8.0, C\#, SQL Server, EF Core, LINQ

\resumeItemListEnd

%----------ILOVETEXT----------
\resumeProject
{iLoveText}
{AI-powered text processing web application with NLP capabilities}
{Dec 2024}
{GitHub: \href{https://github.com/ahmed151515/IloveText}{link}}

\resumeItemListStart

\item \textbf{Application Architecture:} Designed the full application architecture from scratch, separating input handling, API integration, and output rendering into distinct layers

\item \textbf{API Integration:} Integrated the Hugging Face Inference API to apply NLP models for summarization and translation on user-submitted text, with automatic language detection and content moderation

\item \textbf{Backend Development:} Built a Flask backend handling text chunking for long inputs, a translation pipeline, and structured error handling for API and content issues

\item \textbf{Tech Stack:} Python, Flask, Hugging Face Inference API, HTML/CSS

\resumeItemListEnd

\resumeSubHeadingListEnd

\vspace{0mm}

%----------CERTIFICATIONS----------
\section{Certifications}

\resumeSubHeadingListStart

\resumeSubheading
{ALX Software Engineering Program}
{2024}
{ALX Africa}
{Certificate: \href{https://savanna.alxafrica.com/certificates/2syEfHe9Xm}{link}}

\resumeSubHeadingListEnd

\vspace{0mm}

%----------EDUCATION----------
\section{Education}

\resumeSubHeadingListStart

\resumeSubheading
{Bachelor's in Computer Science}
{2022 -- 2026}
{CHI}
{CGPA: 3.23}

\resumeSubHeadingListEnd

\end{document}