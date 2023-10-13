# rav1ator-cli
An easy-to-use CLI utility for working with Av1an, writtin in Bash.

```bash
~ > rav1ator-cli -h
	rAV1ator: CLI Edition_
	Usage: rav1ator-cli [input] [output]
```

rAV1ator CLI Edition can:

- Check if it is installed & up to date on its own without a package manager

- Download AVX2-optimized encoder binaries compiled with `-O3 -flto`` in most cases & allow the user to install them with detailed instructions

- Encode with x264, x265, aomenc, SVT-AV1, or rav1e, set a speed preset, CRF/quality value, FFmpeg parameters, and encoder parameters

- Generate Av1an encoding commands with the user's chosen settings & run them to encode a provided input video to an MKV output.

- Encode from scratch, or resume a previous rav1ator-cli encode

- Engage with rich interactivity features like spinners, prompts, & dropdowns

- Automatically error check binaries with SHA256 hashes for security & convenience

Overall, it aims to provide an easy way to encode videos on the command line with helpful visual feedback. The interactive prompts help users pick encoding settings without needing deep encoding knowledge.

## Installation

Installing rav1ator-cli on its own is as simple as running the following two commands:

```bash
curl -sOJ https://raw.githubusercontent.com/gianni-rosato/rav1ator-cli/main/rav1ator-cli && chmod +x rav1ator-cli
sudo cp rav1ator-cli /usr/local/bin
```

After it is properly installed, it will update itself in the future when updates become available.

Dependencies can be installed on Arch by running the following command:

```bash
yay -Sy rust ffmpeg python mkvtoolnix-cli vapoursynth gum l-smash vapoursynth-plugin-lsmashsource av1an ffms2
```

### Demos

![rav1ator_cli-demo1](./static/rav1ator_cli_demo1.avif)

![rav1ator_cli-demo2](./static/rav1ator_cli_demo2.avif)

If you want to learn more about AV1 encoding, check out [AV1 Encoding for Dummies](https://wiki.x266.mov/blog/av1-encoding-for-dummies)