# Project Polaris Architecture

## Overview

Project Polaris is a content-driven interactive portfolio.

The application separates:

- Content
- Domain logic
- Presentation


## Architecture Principles

### Single Source of Truth

Projects exist as content files.

Everything else is generated.

Content
↓
Processing
↓
Domain Models
↓
UI


### Separation of Concerns

Pages compose.

Components render.

Libraries calculate.

Content describes.


### Growth

Adding a project should require:

1. Create project content file
2. Add assets
3. Deploy

The system should generate the rest.


### Project Structure

project-polaris/


```bash

project-polaris/
├── app/
│   ├── layout.tsx
│   ├── page.tsx
│   ├── projects/
│   └── about/
│
├── components/
│   ├── ui/
│   ├── galaxy/
│   ├── timeline/
│   ├── projects/
│   └── layout/
│
├── content/
│   ├── projects/
│   ├── notebook/
│   └── architecture/
│
├── lib/
│   ├── content/
│   ├── graph/
│   ├── timeline/
│   └── utils/
│
├── types/
│
├── hooks/
│
├── public/
│
└── docs/
```
