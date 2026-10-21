# aicut CLI

[![npm](https://img.shields.io/npm/v/aicut)](https://www.npmjs.com/package/aicut) [![license: MIT](https://img.shields.io/npm/l/aicut)](LICENSE)

> This repository is the public home of the aicut command line: the README, [MODELS.md](MODELS.md), the licence and the issue tracker. The source lives in aicut's private monorepo and the `aicut` package on npm is built and published from there, so there is nothing to build here. Bug reports, model requests and ideas are welcome in [Issues](https://github.com/aicut-pro/cli/issues).

Make AI video, images and audio from your terminal or your coding agent. `aicut` is the command line for [aicut](https://www.aicut.pro), an AI short-form video platform: text to video, image to video, image generation, voiceovers, story episodes and posting, on models like Kling, Veo, Seedance, Wan, Flux and Nano Banana.

Every job is priced before it runs. A person in a terminal is asked y/N; an agent or a script without a terminal is refused unless it passes `--max-tokens`. Nothing is spent by surprise.

## Install

```
npm i -g aicut-cli
aicut login
```

Needs Node 20 or later. `aicut login` opens your browser to sign in to aicut and approve the CLI; on a machine with no browser, `aicut login --no-browser` prints the address to open elsewhere. `aicut account` shows who you are and your token balance.

## Five commands to start

```
# 1. See what you can make, and what it costs
aicut models list --type video

# 2. A picture: --estimate prints the price and charges nothing
aicut generate image --model flux-2-pro --prompt "a lighthouse in a storm, film still" \
  --aspect-ratio 9:16 --resolution 1k --estimate

# 3. Text to video: run it, wait for the result and save it
aicut generate video --model veo-3.1-fast --prompt "a fox running through snow at dawn" \
  --aspect-ratio 9:16 --resolution 720p --duration 4 --wait -o fox.mp4

# 4. Image to video: a local file is uploaded for you
aicut generate video --model seedance-2.0-fast --prompt "the camera slowly pushes in" \
  --start-image ./photo.png --aspect-ratio 9:16 --resolution 720p --duration 5 --wait -o push-in.mp4

# 5. A voiceover
aicut voices --usable-for audio --limit 5
aicut generate audio --model elevenlabs-tts-v3 --text "Welcome to the channel." --voice <voice-id> --wait -o intro.mp3
```

Fields are the model's own published names (`aicut models get <model>` lists them, with the media flags and prices), so a new model needs no new release of the CLI. The full catalogue is in [MODELS.md](https://github.com/aicut-pro/cli/blob/main/MODELS.md). `aicut --help` lists everything else: story episodes, cast and characters, trend formats (`niche`), fake-text chat videos, image stories, upscaling and other transforms, video analysis, trends, and posting to TikTok, YouTube and Instagram.

## How spending works

Creating anything costs tokens from your aicut balance. Every create is quoted first.

- In a terminal you see the price and your balance and answer y/N. `--max-tokens N --yes` skips the question and refuses a quote above N.
- Without a terminal (an agent, a script, CI) the CLI refuses unless you pass `--max-tokens N`; `--yes` counts only together with it. Run with `--estimate` first, read the price, then pass that price as `--max-tokens`.
- Firing a story episode needs `--confirm-fire`, and publishing a post needs `--confirm-publish`.

Top up at https://www.aicut.pro/billing. Add `--json` to any command for the raw API response on stdout; prices and progress go to stderr.

## For coding agents

- Skills for Claude Code, Codex, Cursor and other agents that drive this CLI: `npx skills add aicut-pro/skills` ([aicut-pro/skills](https://github.com/aicut-pro/skills)). They teach the agent to estimate, tell you the price and wait for your go.
- Prefer a hosted connection to a CLI? aicut is also an MCP server: https://www.aicut.pro/mcp

For CI and headless machines, set `AICUT_API_KEY` instead of running `aicut login`. `aicut logout` removes the saved session on this machine only; to sign the CLI out everywhere, remove it under Connected apps at https://www.aicut.pro/account/settings.

## Links

- aicut: https://www.aicut.pro
- Models and prices: [MODELS.md](https://github.com/aicut-pro/cli/blob/main/MODELS.md)
- Skills: https://github.com/aicut-pro/skills
- MCP server: https://www.aicut.pro/mcp
- Issues: https://github.com/aicut-pro/cli/issues

MIT licensed.
