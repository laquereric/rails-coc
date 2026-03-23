# rails-coc

A community effort to help the Rails ecosystem embrace its stated charter. [Ruby on Rails](https://rubyonrails.org/) is built on **Convention Over Configuration** — rails-coc extends that principle into the AI era.

rails-coc publishes quarterly "configuration snapshots" that provide stable, opinionated starting points for Rails development.

## What rails-coc Is

- A community-driven effort to advance the pace of Rails development
- Accepts rapid change as the norm
- Treats configuration stability as a primary value
- Walks a deliberate line between conservative and radical

**On the Conservative Side:**
The successful history of Ruby on Rails "Convention Over Configuration" has created the foundation for a vast amount of software.

**On the Radical Side:**
AI is changing a lot of the software ecosystem. Configuration that doesn't account for this is already behind.

---

## Kickoff: rails-coc-2026-q2

Absent broader community development (to follow), I (Eric Laquer) am kicking things off by proposing a Rails-centric platform that works for the use cases I have in mind:

### 1) Better UI

Many potential collaborators with UX/UI depth have challenged Rails on the basis of its inability to match what other platforms deliver. These folks fall into the "React is all that" and "Swift is all that" camps. I propose the Swift direction:

- [Hotwire Native](https://native.hotwired.dev/) — uses Swift as a wrapper around server-generated HTML
- [ElementaryUI](https://elementary.codes/) — small, efficient components written in Swift running in the browser via WASM

### 2) Better AI

[RubyLLM](https://rubyllm.com/) provides a great LLM "Swiss Army Knife." To build on that as a community, however, standardizing at the model level matters.

I distinguish between the LLM I use for development and the LLMs that application clients use.

My development harness is interesting and I'm continually impressed by what it can accomplish. But that topic is well covered elsewhere, and my LLM costs are amortized over the lifecycle of the products I build. The higher-leverage opportunity is:

**Optimizing the LLMs engaged by application users.** These LLM calls go directly to the bottom line of the enterprise.

- **Path A:** Great UX/UI in a lucrative market, high cost per transaction → fight linear costs the whole way
- **Path B:** Great UX/UI in a lucrative market, low cost per transaction → see profit the whole way

I choose Path B, and I want others who agree to join me here.

#### The Standard Model Choice

Any choice of a standard LLM configuration will be controversial, so I'm going with a **free** choice. Here's what I mean by free — the LLM I'm choosing for rails-coc-2026-q2 is compatible with several deployment models:

1. **Developer** — run it Ollama-style in a container (free)
2. **VPS** — run the container on a VPS (nearly free)
3. **Client-side** — run it via WebGPU on your users' own equipment

The model: [Llama-3.2-1B-Instruct (q4f16_1-MLC)](https://huggingface.co/mlc-ai/Llama-3.2-1B-Instruct-q4f16_1-MLC)

---

## Timeline

It's now March 2026. Between now and June 30, 2026, I'm using this platform to stop shopping and start building.

Some of what I build will be public, some private — I'm interested in building value for myself, not Big Tech.

Please collaborate to advance your own interests along with mine and others'.
