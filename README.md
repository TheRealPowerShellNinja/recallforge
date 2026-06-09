# RecallForge

## Overview

RecallForge is a personal knowledge retention platform designed to help learners retain information through structured review, confidence tracking, and adaptive scheduling.

Unlike traditional flashcard applications that focus primarily on question-and-answer repetition, RecallForge focuses on long-term knowledge retention. The platform is designed to support a wide range of learning content including technical concepts, interview preparation, vocabulary, definitions, Bible verses, language study, certification preparation, and other forms of structured knowledge.

The goal is not simply to help users answer questions correctly today, but to help them retain and recall information weeks, months, and years into the future.

---

## Vision

RecallForge aims to become a flexible knowledge retention platform that adapts to the learner rather than forcing the learner into a predefined workflow.

Users should be able to:

- Capture knowledge quickly
- Organize knowledge over time
- Review information efficiently
- Measure retention objectively
- Track confidence separately from correctness
- Focus study sessions on areas that need reinforcement

Whether the learner is studying CyberArk, Python, AWS, Spanish vocabulary, Greek words, Bible verses, interview questions, or certification material, the same retention engine should support the learning process.

---

## Design Principles

### Retention Over Engagement

RecallForge prioritizes long-term knowledge retention rather than gamification, streaks, or vanity metrics.

Success is measured by what the learner remembers, not by how often they open the application.

### Fast Capture, Rich Organization

Knowledge should be easy to capture.

Organization can be refined later.

Users should be able to create learning items with minimal required information and add categories, tags, notes, and metadata over time.

### Confidence Matters

RecallForge distinguishes between:

- What the learner knew
- How confident the learner felt

A correct answer with low confidence should be treated differently from a correct answer with high confidence.

### Knowledge Decays

Knowledge is not permanent.

Retention must be continuously measured and revalidated over time.

Future versions may include knowledge-status indicators, maintenance scoring, and decaying achievement systems.

### User Configurable, Sensibly Guarded

RecallForge should provide configurable settings while enforcing reasonable guardrails that prevent settings from undermining the review process.

---

## Core Concepts

### Learning Item

A Learning Item is the fundamental unit of knowledge within RecallForge.

Examples include:

- Question and Answer
- Vocabulary Word
- Definition
- Bible Verse
- Foreign Language Translation
- Technical Concept
- Interview Question

### Deck / Pack

A Deck (or Pack) is a collection of Learning Items.

Examples:

- AWS CCP 250 Questions
- CyberArk Interview Questions
- Spanish Vocabulary
- Bible Memory Verses

### Categories

Categories provide structured organization within a deck.

Examples:

- IAM
- S3
- Route 53
- Networking

### Tags

Tags provide flexible filtering and organization across learning items.

Examples:

- interview
- encryption
- weak-area
- review-again

---

## Review Model

RecallForge tracks both objective performance and learner confidence.

### Performance

- Correct
- Incorrect
- Skipped

### Confidence

- Guess
- Low
- Medium
- High

These values may influence future review scheduling and retention scoring.

---

## Session Model

Study sessions are user-driven.

Each user can configure a default session size while retaining the ability to override that value at the start of a session.

Examples:

- Quick review session: 15 items
- Focus session: 50 items
- Long travel session: 250 items

If a session requests more items than are available, RecallForge will automatically use the maximum available items.

---

## MVP Scope

Initial MVP goals include:

- Python-based CLI application
- SQLite database
- Learning Item management
- Deck management
- Categories and basic filtering
- Review sessions
- Confidence tracking
- CSV import support
- JSON import/export support
- Session metrics
- Retention metrics

---

## Future Roadmap

Planned future enhancements may include:

- Docker support
- Web interface
- Multi-device synchronization
- Cloud deployment
- Adaptive review algorithms
- Advanced reporting and analytics
- Knowledge health scoring
- Session review queues
- Import/export templates
- API integrations

---

## Current Status

RecallForge is currently in active design and development.

The project is focused on establishing a solid foundation for long-term knowledge retention, review scheduling, and learning analytics before expanding into web, cloud, and multi-user features.
