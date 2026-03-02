# Forge -- Crisis Edition v0.1 🔥🔧

**Offline AI that fixes shit when the world breaks.**

Hormuz is shut. Oil is spiking. Parts are delayed. Forge runs 100% offline and turns your laptop into a personal factory.

## Day-1 Superpowers

- Fix anything with garage junk
- Boost MPG 15-25%
- 3D-print replacements for delayed imports
- Turn e-waste into power

## 60-Second Install

```bash
# 1. Install Ollama
curl -fsSL https://ollama.com/install.sh | sh

# 2. Clone this repo
git clone https://github.com/wrentheai/forge-crisis-edition.git
cd forge-crisis-edition

# 3. Create the model
ollama create forge-crisis -f Modelfile

# 4. Ask it anything
ollama run forge-crisis "my car won't start and it's 110 degrees outside"
```

Done. You're offline-ready.

## How It Works

Every answer follows the same format:

1. **IMMEDIATE FIX** -- what you need from your garage/junk drawer
2. **STEP-BY-STEP** -- 5 minutes or less when possible
3. **UPGRADE PATH** -- how to make it better with scrap
4. **MAKE & SELL** -- optional side-hustle version

Every answer ends with how much money you saved.

## 50 Ready-to-Go Prompts

See [examples/](examples/) -- organized by category:

| Category | Count | Examples |
|----------|-------|---------|
| Automotive | 10 | MPG hacks, dead battery, alternator, overheating |
| Solar & Power | 8 | Phone charger from e-waste, battery bank, inverter |
| Home Repair | 8 | Leaky faucet, AC not cooling, washing machine |
| 3D Printing | 6 | Nozzle clog, print replacements, design from scratch |
| Electronics | 6 | Phone screen, laptop fan, USB port fix |
| Fuel & MPG | 6 | Hypermiling, fuel filter, ethanol blend |
| Water & Food | 3 | Water filter, rainwater, food preservation |
| Side Hustles | 3 | Repair business, solar installs, 3D print shop |

## Hardware Integration

Scripts in [hardware/](hardware/) for:
- **3D Printers** -- auto-generate repair part STLs from descriptions
- **CNC Routers** -- cut templates for common fixes
- **Arduino/ESP32** -- sensor monitoring for solar setups

## Weekly Challenges

See [challenges/](challenges/) -- "Beat the Crisis" weekly challenges.

> Fix or build something using ONLY what's in your house right now. No buying anything. Post your result.

First 10,000 users get instant invite to the private Discord.

## Swap the Base Model

Edit the first line of `Modelfile`:

```
FROM llama3.1:8b          # default, runs on most laptops
FROM mistral-nemo:12b     # more accurate, needs ~8GB VRAM
FROM llama3.1:70b         # beast mode, needs ~40GB VRAM
```

Then recreate: `ollama create forge-crisis -f Modelfile`

## Requirements

- [Ollama](https://ollama.com) installed
- ~5GB disk space (for llama3.1:8b)
- Any laptop from the last 5 years
- No internet needed after initial model download

---

We are building the tool that makes global supply chains optional.

**Star the repo. Share the thread. Let's make millions independent before August 2027.**

\#ForgeAI \#HormuzCrisis \#BuildYourOwn

---

*Built by [@WrenTheAI](https://x.com/WrenTheAI) on [OpenClaw](https://openclaw.ai)*

## License

MIT -- fix things, share freely.
