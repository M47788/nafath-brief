Version: NAFATH-V3
Track: Software
## Overview  
A government agency is launching a mobile assistant app that lets
citizens ask questions, apply for services, and get directed to the
right government service based on their request. Six IT fields work
together to make this app useful and safe. Software design gives the
app's API clear version numbers so updates do not break older apps.
AI answers citizen questions using official documents instead of
guessing. The iOS app must only connect to servers over secure HTTPS
links. Networking makes sure the app works on both IPv4 and IPv6
networks. Cybersecurity protects the assistant from hidden
instructions that try to control it. Data rules decide when citizen
data must be anonymized or pseudonymized. If one field is weak,
citizens may lose trust in the whole service. This brief explains
each field in turn.
each field in turn.

## Software
Semantic Versioning gives each API release a number in the form
MAJOR.MINOR.PATCH. PATCH increases for bug fixes that do not change
how the API is used. MINOR increases when new features are added in a
backward-compatible way, for example a new optional field showing the
service fee. MAJOR increases when a change breaks old clients, for
example renaming the "status" field in an application response. This
tells mobile developers which updates are safe to accept and which
need code changes.
Resource: Semantic Versioning 2.0.0 - https://semver.org/


## AI

Retrieval-Augmented Generation (RAG) lets the assistant search a
collection of official documents, such as service guides and fee
lists, and give the most relevant parts to the language model before
it answers. The model then answers from these documents instead of
only from what it learned in training. This reduces made-up answers,
lets the assistant show which document it used, and allows the agency
to update answers by updating the documents, without retraining the
model.
Resource: Lewis et al., Retrieval-Augmented Generation for KnowledgeIntensive NLP Tasks - https://arxiv.org/abs/2005.11401
## Mobile
## Networking
## Cybersecurity
## Data
## Misconception in My Track
## Open Question
