---
title: "CV"
---

### About me

I like to tinker with computers/software, learning about good software architecture, and
mathematics. I am captivated by the beauty of functional programming and I am going
down the rabbit hole of learning some category theory for the sake of it.
My current long term goal is to finish developing/deploy my stock trading system.
In the mean time, I am looking for work where I can enhance my functional
programming skills and generate value for the shareholders of the company.

### Technical Skills

A short summery of some of my most relevant technical skills.

#### Programming

| Language | Level        |
| -------- | ------------ |
| C        | Superficial  |
| Fennel   | Proficient   |
| Haskell  | Intermediate |
| Kotlin   | Fluent       |
| Lua      | Fluent       |
| Ocaml    | Basic        |
| Python   | Fluent       |
| Rust     | Basic        |
| Shell    | Fluent       |
| VHDL     | Basic        |

In my spare time I am focusing on improving my skills in Haskell and Ocaml. I am also
keen on trying out Julia, and compare it to Python for data science/machine learning
projects.

#### Markup

| Language | Level      |
| -------- | ---------- |
| HTML     | Proficient |
| LaTeX    | Fluent     |
| markdown | Fluent     |

#### Databases

| Type        | Implementation        |
| ----------- | --------------------- |
| Cache       | Redis                 |
| Graph       | ArangoDB              |
| Index       | Elasticsearch         |
| Message bus | Kafka, SQS            |
| NoSQL       | MongoDB               |
| SQL         | Postgres, TimescaleDB |
| Vector DB   | Qdrant                |

I would like to try out [Nats](https://nats.io/) as a message broker,
[skytable](https://github.com/skytable/skytable) as NoSQL database,
and [meilisearch](https://www.meilisearch.com/) for indexing.

#### Software

Here is a collection of software that I have interacted with that might be
worth mentioning.

| Name       | Level        |
| ---------- | ------------ |
| CircleCI   | Proficient   |
| Docker     | Fluent       |
| Git        | Fluent       |
| Helm       | Proficient   |
| Hugo       | Intermediate |
| Kubernetes | Proficient   |
| Neomutt    | Proficient   |
| Neovim     | Fluent       |
| Tekton     | Proficient   |
| Terraform  | Intermediate |
| Tmux       | Proficient   |

I have plans on learning [Nomad](https://www.nomadproject.io), as this seems to
be a better alternative of k8s. I am also moving to [podman](https://podman.io/)
next time I work with containers in my spare time. I am also keen on working
more with service meshes, to improve my knowledge of their capabilities.

#### Operating Systems

I use Artix Linux as my daily OS. However, I would like to transition to OpenBSD
soon. But, I am a bit afraid of the lack of support for Nvidia GPUs.
Unfortunately, I use macOS for work.

#### Workflow

I use Neovim for all development, together with dwm as a tiling
window manager, and st as the terminal of choice. I am very happy with this
setup, ~~but would like to improve the workflow with increased tmux usage and
git worktrees, à la [ThePrimeagen](https://www.youtube.com/watch?v=GXxvxSlzJdI).~~
I now use worktrees full time, and it is a game changer when it comes to development.
For improving my tmux workflow I now use a popup session which I can easily toggle. I
use this popup sessions to run all time consuming tasks during development in the 
background, such as compiling and running tests.

I build my own keyboard, and I currently have several [ferris sweep](https://github.com/davidphilipbarr/Sweep),
but my latest build is a [Charybdis Nano](https://bastardkb.com/product/charybdis-nano-kit/) and I believe this
to be my endgame when it comes to split keyboards. I also moved on from
qwerty as I do not believe that you should go through life using suboptimal
solutions from the past, just because you cannot bother learning something new.

#### Architecture

Good software is like physics, it should avoid too much complexity, like von
Neumann famously stated, _"With four parameters I can fit an elephant, and with
five I can make him wiggle his trunk"_. I adhere by the [unix
philosophy](http://www.catb.org/esr/writings/taoup/html/ch01s06.html), as well
as the [suckless philosophy](https://suckless.org/philosophy/). I truly believe
that you develop better software by following these principles.

For designing and implementing distributed systems, I really like
the framework presented in the book _The Tao of Microservices_. Web services
should almost be provocatively small, most communication between services
should be asynchronous. It is important to reason and respect separation of concerns.
You should at all cost avoid building a distributed monolith with entangled dependencies.
I also like the idea of designing systems from first principles with defining the
messages first, and not focus on the services from the start.

However, I have now started exploring the idea of "modular monolith", I believe this to be the most
sane approach to building software yet. It keeps the communication simple between modules,
e.g. inter-process instead of network calls, such as http or grpc. It has the benefit of
having the entire source code in one place, making it easier to develop new software
using existing interfaces. If you develop it the right way, modules can easily be
extracted into separate services if necessary. But I see a downside to this approach,
and that is how to deal with the complexity of testing multiple features/branches at
the same time in dev/staging, maybe there is a good way?

#### Machine Learning

I have worked on many machine learning projects, both at work and at home (hobby), ranging
from time series classification, regression, generative models, and machine translation to
name a few. My latest [project](https://github.com/aktersnurra/rag) is a Retrieval
Augmented Generation (RAG) system for my personal library of books and articles. I plan
on extending this to integrate with dmenu, so I can ask questions through the search bar,
which will be pretty cool.

I have also spent quite some time on a OCR [project](https://github.com/aktersnurra/text-recognizer)
where I started with CNN-LSTM based systems to then move on to transformer models that
I have implemented. This has been a crucial project for me, as it has kept me up to date
with the SOTA in transformer architectures, and allowed me to test some of my own ideas out,
most of which were not successful.

#### Miscellaneous

| What      | Level |
| --------- | ----- |
| Soldering | Basic |

### Experience

- Software Engineer. Nexure AB. Aug 2021 -- Present

  - Develop and maintain microservices for payments and subscriptions.
  - Take part in architectural design discussions.
  - Participated in the code review process.
  - Contribute to the infrastructure with updates to k8s resources and AWS
    resource management via Terraform.
  - Monitor logs for bugs in different environments, e.g. staging and
    production.

  _Keywords: Microservices, Kubernetes, Infrastructure, Helm, CI/CD, Kotlin,
  Spring, AWS, Terraform_

- Machine Learning Engineer (Cyber Security). Saab AB. Aug 2020 -- Aug 2021

  - Created data mining pipelines for extracting, cleaning, and creating
    datasets for machine learning models, i.e. train/test sets.
  - Was a driving force in making the system more asynchronous using
    message passing between microservices, by deploying and maintaining a
    Kafka instance. This improve the architecture by allowing multiple
    services to subscribe to incoming sensor data and process the
    information, instead of fetching the data from databases in batches.
  - Developed a modular pipeline for training and evaluating deep learning
    models with different architectures and/or losses. Automatic extraction
    of the best model based on user defined metric, ready for serving.
  - Built and deployed deep learning models for multi-modal trajectory
    predictions in production.
  - Took initiative and deployed and maintained a private Python Package
    Index (PyPI) for all developers. Greatly improving the development
    workflow, e.g. forcing versioning, and reducing/eliminating cross
    dependencies between locally developed Python packages.
  - Developed a graph algorithm for sensor fusion. Deployed it as a
    microservice listing to incoming sensor data. This enabled more complex
    pattern analysis in downstream services.
  - Reduced the docker image size of the Python microservices from ~2 GB
    to ~73 MB by utilizing multistage builds and alpine base images.
  - Built pipelines for CI/CD and packages deployment in Tekton.
  - With my docker images and pipelines we where able to reduce the
    average build times from ~10-30 minutes down to seconds, mostly thanks
    to improved caching capabilities.

  _Keywords: Deep Learning, Python, Microservices, Kubernetes,
  Infrastructure, Helm, CI/CD_

- Machine Learning Engineer (Surveillance). Saab AB. Aug 2018 -- Aug 2020

  - Built simulation software for generating realistic signal
    environments with both radar and/or communication signals. Implemented
    the most common signal encoding for communications, as well as
    basic to SOTA radar modulations. This enabled the team to develop and
    evaluate different machine learning models and ideas.
  - Researched machine learning models in different stages of the radar
    warning receiver, with regards to compute and data limitations.
  - Held in several presentations of machine learning papers in a company
    reading group.
  - Shared the knowledge of implementing and using machine learning to
    multiple business areas within Saab.

  _Keywords: Deep Learning, Signal Processing, Python, VHDL_

### Institutions

- M.Sc., Electrical Engineering. Kungliga Tekniska Högskolan. 2013 -- 2018

  - Specialization in Machine Learning

- Exchange Year. Imperial College London. 2016 -- 2017

- Summer course in Chinese Culture and Language. Dalian University of Technology. 2014

- Economics I. Stockholms universitet. 2013

- Political Science I. Stockholms universitet. 2011

### Languages

| Language | Level  |
| -------- | ------ |
| Swedish  | Native |
| English  | C2     |
