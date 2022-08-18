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
| Fennel   | Fluent       |
| Haskell  | Intermediate |
| Lua      | Fluent       |
| Python   | Fluent       |
| Rust     | Basic        |
| Shell    | Fluent       |
| VHDL     | Basic        |

Haskell is a language I want to master. I find Rust's ownership model
interesting and a language I will explore more.

#### Markup

| Language | Level        |
| -------- | ------------ |
| HTML     | Proficient   |
| LaTeX    | Fluent       |
| markdown | Fluent       |

#### Databases

| Type         | Implementation        |
| ------------ | --------------------- |
| Cache        | Redis                 |
| Graph        | ArangoDB              |
| Index        | Elasticsearch         |
| Message bus  | Kafka, SQS            |
| NoSQL        | MongoDB               |
| SQL          | Postgres, TimescaleDB |

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
| Kubernetes | Proficient   |
| Neomutt    | Proficient   |
| Neovim     | Fluent       |
| Tekton     | Proficient   |
| Terraform  | Intermediate |
| Tmux       | Intermediate |

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
setup, but would like to improve the workflow with increased tmux usage and
git worktrees, à la [ThePrimeagen](https://www.youtube.com/watch?v=GXxvxSlzJdI).
I use a [ferris sweep](https://github.com/davidphilipbarr/Sweep) keyboard with
[Colemak Mod-DH](https://colemakmods.github.io/mod-dh/) layout. I moved on from
qwerty as I do not believe that you should go through life using suboptimal
solutions from the past, just because you cannot bother learning something new.

#### Architecture

Good software is like physics, it should avoid too much complexity, like von
Neumann famously stated, *"With four parameters I can fit an elephant, and with
five I can make him wiggle his trunk"*. I adhere by the [unix
philosophy](http://www.catb.org/esr/writings/taoup/html/ch01s06.html), as well
as the [suckless philosophy](https://suckless.org/philosophy/). I truly believe
that you develop better software by following these principles.

For designing and implementing distributed web service systems, I really like
the framework presented in the book *The Tao of Microservices*. Web services
should almost be provocatively small, most communication between services
should be asynchronous. It is important to reason and respect separation of concerns.
You should at all cost avoid building a distributed monolith with entangled dependencies.

#### Machine Learning

tbc...

#### Signal Processing

tbc...

#### Miscellaneous

| What      | Level |
| --------- | ----- |
| Soldering | Basic |

### Experience

- Nexure AB
  - Software Engineer. Aug 2021 -- Present
    - Develop and maintain microservices for payments and subscriptions.
    - Take part in architectural design discussions.
    - Participated in the code review process.
    - Contribute to the infrastructure with updates to k8s resources and AWS
    resource management via Terraform.
    - Monitor logs for bugs in different environments, e.g. staging and
    production.

    *Keywords: Microservices, Kubernetes, Infrastructure, Helm, CI/CD, Kotlin,
    Spring, AWS, Terraform*

- Saab AB
  - Machine Learning Engineer. Aug 2018 -- Aug 2021
      - Intelligence Application. Aug 2020 -- Aug 2021
        - Created data mining pipelines for extracting, cleaning, and create
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
        - Deployed and maintained a private Python Package Index (PyPI) for all
        developers. Greatly improving the development workflow, e.g. forcing
        versioning, and reducing/eliminating cross dependencies between locally
        developed Python packages.
        - Developed a graph algorithm for sensor fusion. Deployed it as a
        microservice listing to incoming sensor data. This enabled more complex
        pattern analysis in downstream services.
        - Improved the docker image size of the Python microservices from ~2 GB
        to ~73 MB by utilizing multistage builds and alpine base images.
        - Built pipelines for CI/CD and packages deployment in Tekton.
        - With my docker images and pipelines we where able to reduce the
        average build times from ~10-30 minutes down to seconds, mostly thanks
        to improved caching capabilities.

        *Keywords: Deep Learning, Microservices, Kubernetes, Infrastructure,
        Helm, CI/CD*

      - Radar Warning Receiver. Aug 2018 -- Aug 2020
        - Built simulation software for generating realistic signal
        environments with both radar and/or communication signals. Implemented
        the most common signal encoding for communications, as well as
        basic to SOTA radar modulations. This enabled the team to develop and
        evaluate different machine learning models and ideas.
        - Researched machine learning models in different stages of the radar
        warning receiver, and where it would be possible computationally and
        data availability.
        - Held in several presentations of machine learning papers in a company
        reading group.

        *Keywords: Deep Learning, Signal Processing*

### Institutions

- M.Sc., Electrical Engineering. Kungliga Tekniska Högskolan. 2013 -- 2018
    - Major in Machine Learning

- Exchange Year. Imperial College London. 2016 -- 2017

- Summer course in Chinese Culture and Language. Dalian University of Technology. 2014

- Economics I. Stockholms universitet. 2013

- Political Science I. Stockholms universitet. 2011

### Languages

| Language | Level  |
| -------- | ------ |
| Swedish  | Native |
| English  | C2     |
