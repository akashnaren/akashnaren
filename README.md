# Akash

I'm figuring out how agents should use software.

A person gets a screen of buttons. An agent might want something cheaper — a CLI, a structured API, a short form, or a few clicks. Those cost different amounts. I don't think one UI wins for every job.

So I run a small public lab on that question. I write synthetic traces, note a preferred mode, and train a tiny router that picks. The artifacts are lab-made. They are not production data.

The question lives in [agent-ui-metrics](https://github.com/akashnaren/agent-ui-metrics). The pieces:

- [agent-ui-sft](https://huggingface.co/datasets/akashnaren/agent-ui-sft) — multi-turn tool traces, each tagged with a UI mode
- [agent-ui-human](https://huggingface.co/datasets/akashnaren/agent-ui-human) — one request, a preferred UI, and a short why
- [agent-ui-mode-pairs](https://huggingface.co/datasets/akashnaren/agent-ui-mode-pairs) — this mode over that one
- [agent-ui-efficiency-scores](https://huggingface.co/datasets/akashnaren/agent-ui-efficiency-scores) — a small lab score table
- [ui-mode-router](https://huggingface.co/akashnaren/ui-mode-router) · [demo](https://huggingface.co/spaces/akashnaren/agent-ui-router) — a toy sklearn router

They're in the [Agent UI lab](https://huggingface.co/collections/akashnaren/agent-ui-lab-6a9a8e06fec692165b0b3c07) collection.

[site](https://akashnaren.github.io/) · [bot](https://akashnaren.github.io/bot) · [cursor](https://cursor.com/@akashpn) · [x](https://x.com/akashpn)
