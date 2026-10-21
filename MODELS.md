# aicut models

The AI video, image and audio models you can run from the [aicut CLI](README.md), generated from `GET https://api.aicut.pro/v1/models` on 2026-10-21: 37 models, priced in aicut tokens.

Run `aicut models list` or `aicut models get <model>` for the live catalogue, and `aicut generate <video|image|audio> --model <model> ... --estimate` to see the exact price of a request before you spend anything. A new model needs no CLI release.

## Image models

| Model | Price | Aspect ratios |
| --- | --- | --- |
| [nano-banana-2](#nano-banana-2) | 0.3 to 0.6 tokens | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| [nano-banana-2.1](#nano-banana-21) | 0.3 to 0.6 tokens | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| [nano-banana-2-lite](#nano-banana-2-lite) | 0.2 tokens | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| [nano-banana-pro](#nano-banana-pro) | 0.6 to 1.2 tokens | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| [flux-2-pro](#flux-2-pro) | 0.1 to 0.2 tokens | 3:4, 4:3, 9:16, 16:9, 1:1, 2:3, 3:2 |
| [flux-3-image](#flux-3-image) | 0.25 to 2.5 tokens | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| [seedream-4.5](#seedream-45) | 0.2 tokens | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| [seedream-5](#seedream-5) | 0.2 to 0.4 tokens | 3:4, 4:3, 9:16, 16:9, 1:1, 2:3, 3:2 |
| [gpt-image-2.0](#gpt-image-20) | 0.1 to 2 tokens | 2:3, 3:2, 3:4, 4:3, 1:1, 9:16, 16:9, 21:9 |
| [gpt-image-2.5](#gpt-image-25) | 0.1 to 2 tokens | 2:3, 3:2, 3:4, 4:3, 1:1, 9:16, 16:9, 21:9 |

### nano-banana-2

- Price: 0.3 to 0.6 tokens
- Aspect ratios: 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2
- Resolutions: 1k, 2k, 4k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 20000 |
| `--aspect-ratio` | string | yes | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| `--resolution` | string | yes | 1k, 2k, 4k |

### nano-banana-2.1

- Price: 0.3 to 0.6 tokens
- Aspect ratios: 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2
- Resolutions: 1k, 2k, 4k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 20000 |
| `--aspect-ratio` | string | yes | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| `--resolution` | string | yes | 1k, 2k, 4k |

### nano-banana-2-lite

- Price: 0.2 tokens
- Aspect ratios: 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2
- Resolutions: 1k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 20000 |
| `--aspect-ratio` | string | yes | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| `--resolution` | string | yes | 1k |

### nano-banana-pro

- Price: 0.6 to 1.2 tokens
- Aspect ratios: 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2
- Resolutions: 1k, 2k, 4k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 10000 |
| `--aspect-ratio` | string | yes | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| `--resolution` | string | yes | 1k, 2k, 4k |

### flux-2-pro

- Price: 0.1 to 0.2 tokens
- Aspect ratios: 3:4, 4:3, 9:16, 16:9, 1:1, 2:3, 3:2
- Resolutions: 1k, 2k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 3:4, 4:3, 9:16, 16:9, 1:1, 2:3, 3:2 |
| `--resolution` | string | yes | 1k, 2k |

### flux-3-image

- Price: 0.25 to 2.5 tokens
- Aspect ratios: 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2
- Resolutions: 1k, 2k, 4k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| `--resolution` | string | yes | 1k, 2k, 4k |

### seedream-4.5

- Price: 0.2 tokens
- Aspect ratios: 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 3000 |
| `--aspect-ratio` | string | yes | 3:4, 4:3, 9:16, 16:9, 21:9, 1:1, 2:3, 3:2 |
| `--resolution` | string | yes | 2k, 4k |

### seedream-5

- Price: 0.2 to 0.4 tokens
- Aspect ratios: 3:4, 4:3, 9:16, 16:9, 1:1, 2:3, 3:2
- Resolutions: 1k, 2k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 3000 |
| `--aspect-ratio` | string | yes | 3:4, 4:3, 9:16, 16:9, 1:1, 2:3, 3:2 |
| `--resolution` | string | yes | 1k, 2k |

### gpt-image-2.0

- Price: 0.1 to 2 tokens
- Aspect ratios: 2:3, 3:2, 3:4, 4:3, 1:1, 9:16, 16:9, 21:9
- Resolutions: 1k, 2k, 4k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 32000 |
| `--aspect-ratio` | string | yes | 2:3, 3:2, 3:4, 4:3, 1:1, 9:16, 16:9, 21:9 |
| `--resolution` | string | yes | 1k, 2k, 4k |
| `--quality` | string | yes | low, medium, high |

### gpt-image-2.5

- Price: 0.1 to 2 tokens
- Aspect ratios: 2:3, 3:2, 3:4, 4:3, 1:1, 9:16, 16:9, 21:9
- Resolutions: 1k, 2k, 4k
- Inputs, a URL or a local file: `--images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 20000 |
| `--aspect-ratio` | string | yes | 2:3, 3:2, 3:4, 4:3, 1:1, 9:16, 16:9, 21:9 |
| `--resolution` | string | yes | 1k, 2k, 4k |
| `--quality` | string | yes | low, medium, high, xhigh, max |
| `--variant` | string | no | flare, sunburst |

## Video models

| Model | Price | Aspect ratios |
| --- | --- | --- |
| [ltx-2-pro](#ltx-2-pro) | 3 to 7 tokens | 16:9, 9:16 |
| [ltx-2-fast](#ltx-2-fast) | 2.4 to 24 tokens | 16:9, 9:16 |
| [grok-imagine](#grok-imagine) | 0.3 to 7.5 tokens | 16:9, 9:16, 1:1, 2:3, 3:2 |
| [veo-3.1-fast](#veo-31-fast) | 2 tokens | 16:9, 9:16 |
| [veo-3.1](#veo-31) | 5 tokens | 16:9, 9:16 |
| [veo-3.1-lite](#veo-31-lite) | 1 tokens | 16:9, 9:16 |
| [wan-2.2](#wan-22) | 1.6 tokens | 1:1, 16:9, 9:16 |
| [wan-2.2-turbo](#wan-22-turbo) | 0.4 tokens | 16:9, 9:16 |
| [kling-3.0](#kling-30) | 1.5 to 15 tokens | 1:1, 16:9, 9:16 |
| [kling-3.0-turbo](#kling-30-turbo) | 1.2 to 9 tokens | 1:1, 16:9, 9:16 |
| [seedance-2.0](#seedance-20) | 1.4 to 93.75 tokens | 1:1, 21:9, 4:3, 3:4, 16:9, 9:16 |
| [seedance-2.0-fast](#seedance-20-fast) | 1.2 to 9 tokens | 1:1, 21:9, 4:3, 3:4, 16:9, 9:16 |
| [seedance-2.0-mini](#seedance-20-mini) | 0.8 to 6 tokens | 1:1, 21:9, 4:3, 3:4, 16:9, 9:16 |
| [seedance-2.5](#seedance-25) | 1.92 to 76.8 tokens | 1:1, 21:9, 4:3, 3:4, 16:9, 9:16 |
| [kling-2.5-pro](#kling-25-pro) | 1.5 to 3 tokens | 1:1, 16:9, 9:16 |
| [kling-2.6](#kling-26) | 1.25 to 5 tokens | 1:1, 16:9, 9:16 |
| [wan-2.7](#wan-27) | 0.8 to 6 tokens | 16:9, 9:16, 1:1, 4:3, 3:4 |
| [wan-3.0](#wan-30) | 0.4 to 24 tokens | 16:9, 9:16, 1:1, 4:3, 3:4 |
| [wan-3.0-prime](#wan-30-prime) | 0.6 to 33 tokens | 16:9, 9:16, 1:1, 4:3, 3:4 |
| [flux-3](#flux-3) | 3.5 to 24 tokens | 16:9, 9:16, 1:1, 4:3, 3:4 |
| [minimax-h3-max](#minimax-h3-max) | 1 to 9 tokens | 16:9, 9:16, 1:1, 4:3, 3:4 |

### ltx-2-pro

- Price: 3 to 7 tokens
- Aspect ratios: 16:9, 9:16
- Durations (seconds): 6, 8, 10
- Resolutions: 720p, 1080p
- Inputs, a URL or a local file: `--start-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16 |
| `--resolution` | string | yes | 720p, 1080p |
| `--duration` | number | yes | 6, 8, 10 |

### ltx-2-fast

- Price: 2.4 to 24 tokens
- Aspect ratios: 16:9, 9:16
- Durations (seconds): 6, 8, 10, 12, 14, 16, 18, 20
- Resolutions: 720p, 1080p, 1440p, 2160p
- Inputs, a URL or a local file: `--start-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16 |
| `--resolution` | string | yes | 720p, 1080p, 1440p, 2160p |
| `--duration` | number | yes | 6, 8, 10, 12, 14, 16, 18, 20 |

### grok-imagine

- Price: 0.3 to 7.5 tokens
- Aspect ratios: 16:9, 9:16, 1:1, 2:3, 3:2
- Durations (seconds): 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
- Resolutions: 720p, 1080p
- Inputs, a URL or a local file: `--start-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 4096 |
| `--aspect-ratio` | string | yes | 16:9, 9:16, 1:1, 2:3, 3:2 |
| `--resolution` | string | no | 720p, 1080p |
| `--duration` | number | yes | 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 |

### veo-3.1-fast

- Price: 2 tokens
- Aspect ratios: 16:9, 9:16
- Durations (seconds): 4, 6, 8
- Resolutions: 720p, 1080p
- Inputs, a URL or a local file: `--start-image`, `--end-image`, `--reference-images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 50000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16 |
| `--resolution` | string | yes | 720p, 1080p |
| `--duration` | number | yes | 4, 6, 8 |

### veo-3.1

- Price: 5 tokens
- Aspect ratios: 16:9, 9:16
- Durations (seconds): 4, 6, 8
- Resolutions: 720p, 1080p
- Inputs, a URL or a local file: `--start-image`, `--end-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 50000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16 |
| `--resolution` | string | yes | 720p, 1080p |
| `--duration` | number | yes | 4, 6, 8 |

### veo-3.1-lite

- Price: 1 tokens
- Aspect ratios: 16:9, 9:16
- Durations (seconds): 4, 6, 8
- Resolutions: 720p, 1080p
- Inputs, a URL or a local file: `--start-image`, `--end-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 50000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16 |
| `--resolution` | string | yes | 720p, 1080p |
| `--duration` | number | yes | 4, 6, 8 |

### wan-2.2

- Price: 1.6 tokens
- Aspect ratios: 1:1, 16:9, 9:16
- Inputs, a URL or a local file: `--start-image`, `--end-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 1:1, 16:9, 9:16 |

### wan-2.2-turbo

- Price: 0.4 tokens
- Aspect ratios: 16:9, 9:16
- Inputs, a URL or a local file: `--start-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16 |

### kling-3.0

- Price: 1.5 to 15 tokens
- Aspect ratios: 1:1, 16:9, 9:16
- Durations (seconds): 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
- Resolutions: 720p, 1080p
- Inputs, a URL or a local file: `--start-image`, `--end-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 2500 |
| `--aspect-ratio` | string | yes | 1:1, 16:9, 9:16 |
| `--resolution` | string | yes | 720p, 1080p |
| `--duration` | number | yes | 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 |
| `--audio` | bool | no |  |

### kling-3.0-turbo

- Price: 1.2 to 9 tokens
- Aspect ratios: 1:1, 16:9, 9:16
- Durations (seconds): 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
- Resolutions: 720p, 1080p
- Inputs, a URL or a local file: `--start-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 2500 |
| `--aspect-ratio` | string | yes | 1:1, 16:9, 9:16 |
| `--resolution` | string | yes | 720p, 1080p |
| `--duration` | number | yes | 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 |

### seedance-2.0

- Price: 1.4 to 93.75 tokens
- Aspect ratios: 1:1, 21:9, 4:3, 3:4, 16:9, 9:16
- Durations (seconds): 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
- Resolutions: 480p, 720p, 1080p, 4k
- Inputs, a URL or a local file: `--start-image`, `--end-image`, `--reference-images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 1:1, 21:9, 4:3, 3:4, 16:9, 9:16 |
| `--resolution` | string | yes | 480p, 720p, 1080p, 4k |
| `--duration` | number | yes | 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 |
| `--audio` | bool | no |  |

### seedance-2.0-fast

- Price: 1.2 to 9 tokens
- Aspect ratios: 1:1, 21:9, 4:3, 3:4, 16:9, 9:16
- Durations (seconds): 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
- Resolutions: 480p, 720p
- Inputs, a URL or a local file: `--start-image`, `--end-image`, `--reference-images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 1:1, 21:9, 4:3, 3:4, 16:9, 9:16 |
| `--resolution` | string | yes | 480p, 720p |
| `--duration` | number | yes | 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 |
| `--audio` | bool | no |  |

### seedance-2.0-mini

- Price: 0.8 to 6 tokens
- Aspect ratios: 1:1, 21:9, 4:3, 3:4, 16:9, 9:16
- Durations (seconds): 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
- Resolutions: 480p, 720p
- Inputs, a URL or a local file: `--start-image`, `--end-image`, `--reference-images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 20000 |
| `--aspect-ratio` | string | yes | 1:1, 21:9, 4:3, 3:4, 16:9, 9:16 |
| `--resolution` | string | yes | 480p, 720p |
| `--duration` | number | yes | 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 |
| `--audio` | bool | no |  |

### seedance-2.5

- Price: 1.92 to 76.8 tokens
- Aspect ratios: 1:1, 21:9, 4:3, 3:4, 16:9, 9:16
- Durations (seconds): 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30
- Resolutions: 480p, 720p, 1080p
- Inputs, a URL or a local file: `--start-image`, `--end-image`, `--reference-images`, `--reference-audios`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 30000 |
| `--aspect-ratio` | string | yes | 1:1, 21:9, 4:3, 3:4, 16:9, 9:16 |
| `--resolution` | string | yes | 480p, 720p, 1080p |
| `--duration` | number | yes | 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30 |
| `--audio` | bool | no |  |

### kling-2.5-pro

- Price: 1.5 to 3 tokens
- Aspect ratios: 1:1, 16:9, 9:16
- Durations (seconds): 5, 10
- Inputs, a URL or a local file: `--start-image`, `--end-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 2500 |
| `--aspect-ratio` | string | yes | 1:1, 16:9, 9:16 |
| `--duration` | number | yes | 5, 10 |

### kling-2.6

- Price: 1.25 to 5 tokens
- Aspect ratios: 1:1, 16:9, 9:16
- Durations (seconds): 5, 10
- Inputs, a URL or a local file: `--start-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 2500 |
| `--aspect-ratio` | string | yes | 1:1, 16:9, 9:16 |
| `--duration` | number | yes | 5, 10 |
| `--audio` | bool | no |  |

### wan-2.7

- Price: 0.8 to 6 tokens
- Aspect ratios: 16:9, 9:16, 1:1, 4:3, 3:4
- Durations (seconds): 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
- Inputs, a URL or a local file: `--start-image`, `--end-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16, 1:1, 4:3, 3:4 |
| `--resolution` | string | yes | 720p, 1080p |
| `--duration` | number | yes | 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 |

### wan-3.0

- Price: 0.4 to 24 tokens
- Aspect ratios: 16:9, 9:16, 1:1, 4:3, 3:4
- Durations (seconds): 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30
- Resolutions: 480p, 720p, 1080p
- Inputs, a URL or a local file: `--start-image`, `--end-image`, `--reference-images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16, 1:1, 4:3, 3:4 |
| `--resolution` | string | yes | 480p, 720p, 1080p |
| `--duration` | number | yes | 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30 |

### wan-3.0-prime

- Price: 0.6 to 33 tokens
- Aspect ratios: 16:9, 9:16, 1:1, 4:3, 3:4
- Durations (seconds): 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30
- Resolutions: 480p, 720p, 1080p
- Inputs, a URL or a local file: `--start-image`, `--end-image`, `--reference-images`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16, 1:1, 4:3, 3:4 |
| `--resolution` | string | yes | 480p, 720p, 1080p |
| `--duration` | number | yes | 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30 |

### flux-3

- Price: 3.5 to 24 tokens
- Aspect ratios: 16:9, 9:16, 1:1, 4:3, 3:4
- Durations (seconds): 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20
- Resolutions: 720p, 1080p
- Inputs, a URL or a local file: `--start-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16, 1:1, 4:3, 3:4 |
| `--resolution` | string | yes | 720p, 1080p |
| `--duration` | number | yes | 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20 |

### minimax-h3-max

- Price: 1 to 9 tokens
- Aspect ratios: 16:9, 9:16, 1:1, 4:3, 3:4
- Durations (seconds): 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
- Resolutions: 480p, 768p, 1080p
- Inputs, a URL or a local file: `--start-image`, `--end-image`

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 5000 |
| `--aspect-ratio` | string | yes | 16:9, 9:16, 1:1, 4:3, 3:4 |
| `--resolution` | string | yes | 480p, 768p, 1080p |
| `--duration` | number | yes | 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15 |

## Audio models

| Model | Price | Aspect ratios |
| --- | --- | --- |
| [elevenlabs-tts-v2](#elevenlabs-tts-v2) | 0.48 tokens per 1000 characters | - |
| [elevenlabs-tts-v3](#elevenlabs-tts-v3) | 0.48 tokens per 1000 characters | - |
| [elevenlabs-tts-v4](#elevenlabs-tts-v4) | 0.48 tokens per 1000 characters | - |
| [elevenlabs-music](#elevenlabs-music) | 3.2 tokens per 60000 milliseconds | - |
| [suno-v6](#suno-v6) | 0.5 tokens | - |
| [elevenlabs-sfx](#elevenlabs-sfx) | 0.015 tokens per 1 seconds | - |

### elevenlabs-tts-v2

- Price: 0.48 tokens per 1000 characters

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--text` | string | yes | up to 50000 |
| `--voice` | string | yes | up to 256 |
| `--stability` | number | no | 0 to 1 |
| `--similarity-boost` | number | no | 0 to 1 |
| `--style` | number | no | 0 to 1 |
| `--speed` | number | no | 0.7 to 1.2 |

### elevenlabs-tts-v3

- Price: 0.48 tokens per 1000 characters

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--text` | string | yes | up to 50000 |
| `--voice` | string | yes | up to 256 |
| `--stability` | number | no | 0 to 1 |

### elevenlabs-tts-v4

- Price: 0.48 tokens per 1000 characters

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--text` | string | yes | up to 10000 |
| `--voice` | string | yes | up to 256 |
| `--stability` | number | no | 0 to 1 |
| `--similarity-boost` | number | no | 0 to 1 |

### elevenlabs-music

- Price: 3.2 tokens per 60000 milliseconds

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | yes | up to 4100 |
| `--length-ms` | number | no | 3000 to 600000 |
| `--force-instrumental` | bool | no |  |

### suno-v6

- Price: 0.5 tokens

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--prompt` | string | no | up to 3000 |
| `--custom-mode` | bool | no |  |
| `--music-style` | string | yes | up to 1000 |
| `--lyrics` | string | no | up to 5000 |
| `--title` | string | no | up to 80 |
| `--vocal-gender` | string | no | m, f |
| `--duration-seconds` | number | no | 10 to 360 |

### elevenlabs-sfx

- Price: 0.015 tokens per 1 seconds

| Flag | Type | Required | Values |
| --- | --- | --- | --- |
| `--text` | string | yes | up to 5000 |
| `--duration` | number | no | 0.5 to 30 |
| `--prompt-influence` | number | no | 0 to 1 |
| `--loop` | bool | no |  |
