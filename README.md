<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6C3EF4,100:00D4FF&height=220&section=header&text=Tousif%20Rahman%20Anto&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Software%20Engineer%20%7C%20CSE%20Graduate%2C%20BRAC%20University&descAlignY=58&descSize=18" width="100%"/>

<a href="https://github.com/Tousifrahmananto">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=800&color=00D4FF&center=true&vCenter=true&multiline=true&width=700&height=90&lines=Full-stack+web+apps+in+MERN%2C+Next.js+and+Django;LLM+features+with+fallbacks+and+key+rotation;Open+to+junior+software+engineering+roles" alt="Typing SVG" />
</a>

</div>

<br/>

I'm Tousif, a software engineer from Dhaka, Bangladesh. I finished my Computer Science and Engineering degree at BRAC University in September 2026 and I'm looking for junior full-stack or backend roles. Most of my work is web software: Node, Django and Next.js backends, a React or Next.js frontend, and more recently LLM APIs, multi-tenant data and real-time updates.

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:6C3EF4,100:00D4FF&height=3&width=100%" width="100%"/>

## Right now

I'm applying for junior software engineering jobs, so the projects below are the ones I'd point an interviewer to first. I'm still adding to CodeSwitch, mostly on the backend side (multi-tenancy, audit logging, observability). I also run AFK Productions, a 25-person esports production crew, and the tournament platform below was built for it.

My undergraduate thesis was titled "Toward a Self-Evolving Conversational AI: Integrating Generative NLP with Psychological Modeling." It fine-tuned four 7B open models with LoRA, ran them locally, and compared them using alignment metrics I wrote for inference time. Before graduating I served on the Global Admissions Committee for the Millennium Fellowship (UNAI and MCN).

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:6C3EF4,100:00D4FF&height=3&width=100%" width="100%"/>

## Stack

<p align="left">
<img src="https://skillicons.dev/icons?i=ts,js,py,cpp,java,php,dart,html,css,react,nextjs,vite,tailwind,threejs,flutter,nodejs,express,django,mongodb,postgres,mysql,supabase,docker,git,github,vercel,figma&perline=9" />
</p>

On the AI side I've worked with the OpenAI API, Groq, Gemini and LangChain. For real-time features I use Socket.IO.

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:6C3EF4,100:00D4FF&height=3&width=100%" width="100%"/>

## Projects

### [CodeSwitch](https://github.com/Tousifrahmananto/CodeSwitch)

Converts code between Python, C, C++, Java and JavaScript. It sends the request to an LLM (Groq, OpenAI or Gemini) and rotates API keys when one fails, and if every key is exhausted it falls back to a rule-based regex engine so the app still returns something. It can also run the converted code in a sandbox, explain what changed, and share a conversion as a public link. There's a learning section with quizzes, a per-user file manager and an admin panel. Auth uses httpOnly JWT cookies with token rotation and brute-force lockout. Multi-tenancy, role-based access and OpenTelemetry, Prometheus and Grafana monitoring sit on top of that. The backend runs on Railway.

Stack: Django, Django REST Framework, React 18, TypeScript, Monaco Editor

### [MediPay](https://github.com/Tousifrahmananto/MediPay) · [live demo](https://saas-project-client-beta.vercel.app)

A multi-tenant billing portal for hospitals and clinics. A patient encounter collects department charges, the charges become an invoice, and the invoice can be paid in parts through SSLCOMMERZ (sandbox mode) or recorded as cash or bank payments. It also handles refunds, reconciliation, PDF invoices and receipts, appointments, contracts with e-signatures, claims and a full audit log. The parts I spent the most time on are the ones where money is involved: decimal arithmetic instead of floats, MongoDB transactions when charges are turned into an invoice or a payment settles, immutable invoice snapshots, and role checks repeated on the backend for every protected route. Eight roles, from owner and billing admin to cashier and doctor.

Stack: React 19, Vite, Express 5, TypeScript, MongoDB, Zod, Vitest. Vercel for the frontend and Render for the API.

### [AFK Productions Platform](https://github.com/Tousifrahmananto/AFK_PRODUCTIONS) · [live](https://afk-productions-frontend.vercel.app)

An esports tournament platform built for the AFK Productions crew. Admins create tournaments, teams and players register, and the platform generates single elimination, double elimination or round robin brackets, with byes handled automatically and winners advanced when an admin records a result. It also covers leaderboards, match stats, media galleries and notifications that arrive over WebSockets.

Stack: React, Node.js, Express, MongoDB, Socket.IO, Tailwind CSS

### [The Archive](https://github.com/Tousifrahmananto/The-Archive) · [live](https://the-archive-pdf.vercel.app)

A private PDF vault. Users sign in through Supabase, upload PDFs up to 20 MB, search their own library, preview documents in the browser and share a link. Every file API checks the bearer token and is rate limited, and files are stored under per-user paths so one user can't list another's documents. I wrote the requirements spec for it before building.

Stack: Next.js (App Router), React 19, Supabase Auth, Vercel Blob

### Secure Notes · [API](https://github.com/Tousifrahmananto/care_guide_backend) · [frontend](https://github.com/Tousifrahmananto/care_guide_frontend) · [live](https://care-guide-notes.vercel.app)

A note-taking app where users keep private notes and can publish public posts. Admins manage accounts and read every note. The API uses MongoDB transactions for account deletion and note creation, indexes only the fields that are queried, paginates every list, and has aggregation views that group users by interest and pull one author's public posts. The frontend is plain HTML, CSS and JavaScript with no build step.

Stack: Express, MongoDB, Mongoose, JWT, bcrypt. API on Render, frontend on Vercel.

### [Game Physics Lab](https://github.com/Tousifrahmananto/Game-Physics-Lab)

A browser tool for trying out how game objects behave before rebuilding that behaviour in an engine. You can add primitives or upload .glb, .gltf and .obj models, assign materials, and run one of eleven simulations: throw, drop, bounce, wind tunnel, fire, water tank, stack stability, rolling ramp, sliding ramp, explosion and a gravity chamber. Explosions break objects into fragments that are simulated separately. Everything runs client-side, and it is still a prototype (v0.1.0).

Stack: React, Three.js, Cannon-es

### [Portfolio](https://www.tousifrahmananto.me) · [repo](https://github.com/Tousifrahmananto/TOUSIFRAHMANANTOPORT)

My personal site. The build prerenders the home page and each project page, and generates the sitemap and structured data for search engines.

Stack: React, TypeScript, Vite

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:6C3EF4,100:00D4FF&height=3&width=100%" width="100%"/>

## Smaller projects

[Dhaka Bus Tracker](https://github.com/Tousifrahmananto/credosis_backend_task) is a backend demo built one endpoint at a time: routes, bus locations with stale-reading flags, and GPS updates authenticated with a separate bearer token per bus. It runs on Node.js with SQLite and has Swagger docs. All the data is simulated.

[The Chuckle Chronicles](https://github.com/Tousifrahmananto/The-Chuckle-Chronicles) is a blog written in plain PHP and MySQL, with registration and login, categories, comments, likes and an admin panel.

[Workshop Appointments](https://github.com/Tousifrahmananto/Workshop-Appointments) is a car workshop booking system in PHP and MySQL. Customers book through a form and an admin logs in to view and edit appointments.

[Geo Entity Manager](https://github.com/Tousifrahmananto/Geo-Entity-Manager) is a Flutter app from my mobile development course. It uses flutter_map, device location and the image picker.

LMS Platform is a learning management system with four roles (admin, content manager, instructor, student), enrollment, progress tracking, auto-graded quizzes and a blog with drafts. The frontend is Next.js on Vercel and the backend is Strapi on Railway.

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:6C3EF4,100:00D4FF&height=3&width=100%" width="100%"/>

## GitHub stats

<div align="center">
<img height="165em" src="https://github-readme-stats.shion.dev/api?username=Tousifrahmananto&theme=radical&hide_border=true&include_all_commits=true&count_private=true"/>
<img height="165em" src="https://github-readme-stats.shion.dev/api/top-langs/?username=Tousifrahmananto&theme=radical&hide_border=true&layout=compact&include_all_commits=true&count_private=true"/>
</div>

<div align="center">
<img src="https://streak-stats.demolab.com/?user=Tousifrahmananto&theme=radical&hide_border=true" alt="GitHub Streak"/>
</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:6C3EF4,100:00D4FF&height=3&width=100%" width="100%"/>

## Contact

<div align="center">

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tousif.rahman.anto@g.bracu.ac.bd)
[![Website](https://img.shields.io/badge/Website-6C3EF4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://www.tousifrahmananto.me)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Tousifrahmananto)
<!-- Add your LinkedIn here:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/YOUR-HANDLE)
-->

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00D4FF,100:6C3EF4&height=120&section=footer" width="100%"/>
