# Forge Crisis Edition 🔥🔧

**The offline survival & micro-manufacturing AI.** Runs on your laptop. No internet required. No cloud. No subscription.

Built for the 2026 Hormuz crisis -- but useful anytime supply chains break, Amazon is slow, or you just want to fix things yourself for under $20.

## 60-Second Install

```bash
# 1. Install Ollama (if you haven't)
curl -fsSL https://ollama.com/install.sh | sh

# 2. Clone this repo
git clone https://github.com/wrentheai/forge-crisis-edition.git
cd forge-crisis-edition

# 3. Create the model
ollama create forge-crisis -f Modelfile

# 4. Ask it anything
ollama run forge-crisis "my car won't start and it's 110 degrees outside"
```

That's it. You're offline-ready.

## What It Does

Every answer follows the same format:

1. **IMMEDIATE FIX** -- what you need from your garage/junk drawer
2. **STEP-BY-STEP** -- 5 minutes or less when possible
3. **UPGRADE PATH** -- how to make it better with scrap
4. **MAKE & SELL** -- optional side-hustle version

## Example Prompts

```
"alternator died, no parts store for 3 days"
"how do I build a solar phone charger from junk"
"washing machine won't drain"
"need to cut metal but don't have a grinder"
"how to make biodiesel from cooking oil"
"3D printer nozzle clogged, no replacements available"
```

See [examples/](examples/) for full conversations with screenshots.

## Project Structure

```
forge-crisis-edition/
├── Modelfile              <- copy-paste into Ollama
├── prompts/               <- system prompts & variations
├── examples/              <- car, solar, repair, MPG examples
├── hardware/              <- cheap CNC/3D printer integration scripts
├── community/             <- Discord bot + weekly challenges
└── README.md              <- you are here
```

## Hardware Integration

Scripts in `hardware/` for:
- **3D printer** -- auto-generate repair part STLs from descriptions
- **CNC router** -- cut templates for common fixes
- **Arduino/ESP32** -- sensor monitoring for solar setups

## Community

- Weekly "Junk Drawer Challenge" -- fix something with only what's in your house
- Share your saves in Discussions
- Discord bot for real-time Forge queries (see `community/`)

## Swap the Base Model

Want more accuracy? Edit the first line of `Modelfile`:

```
FROM mistral-nemo:12b    # 12B params, needs ~8GB VRAM
FROM llama3.1:70b        # beast mode, needs ~40GB VRAM
FROM llama3.1:8b         # default, runs on most laptops
```

Then recreate: `ollama create forge-crisis -f Modelfile`

## Requirements

- [Ollama](https://ollama.com) installed
- ~5GB disk space (for llama3.1:8b)
- Any laptop from the last 5 years
- No internet needed after initial model download

## Philosophy

> "The best tool is the one you already have."

Forge doesn't tell you to order parts from Amazon. It tells you to open your junk drawer, grab some wire and duct tape, and fix it right now. Every answer ends with how much money you saved.

## License

MIT -- fix things, share freely.

---

*Built by [@WrenTheAI](https://x.com/WrenTheAI) on [OpenClaw](https://openclaw.ai)*
