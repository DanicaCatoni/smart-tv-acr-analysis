# smart-tv-acr-analysis

Measuring what a Sony smart TV's automatic content recognition (ACR) sends home, using the NSF-funded SPHERE IoT testbed

Privacy analysis of automatic content recognition (ACR) on a Sony smart TV, built at the **IoT Privacy Hackathon** (Boston, Oct 2026).

Using the NSF-funded **SPHERE** IoT testbed, I ran remote experiments on the TV, automating IR control through a command-line interface while switching between HDMI and over-the-air inputs. I captured the TV's live network traffic and analysed it to see when ACR data is collected, where it goes, and what that means for viewers' privacy.

## Method
1. **Control:** automate the TV over IR from the CLI (power, inputs, channels).
2. **Vary inputs:** switch between HDMI and over-the-air sources to trigger ACR.
3. **Capture:** record traffic with Wireshark / PCAP files.
4. **Analyse:** Python CLI tools to group traffic by destination, timing and volume.

## Findings
_Add a short summary: which domains the TV contacts, how often, and whether ACR runs on HDMI inputs too._

## Tools
Python, Wireshark, PCAP, SPHERE testbed, IR control CLI

## Repository layout
```
scripts/    device control and capture automation
analysis/   traffic analysis scripts and figures
docs/       write-up and slides
```

> Raw PCAP files are excluded by `.gitignore` because they can contain identifying data.

## Author
Danica Catoni, Boston University · [danicacatoni.github.io](https://danicacatoni.github.io)
