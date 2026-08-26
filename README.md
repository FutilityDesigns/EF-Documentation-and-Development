# EF-Documentation-and-Development
Documentation on the Reverse Engineering efforts into the Canon EF Protocol

 This repository holds the raw data, analysis scripts, and final summaries generated during my work reverse engineering the Canon EF Protocol. Findings are published here with the aim to share the knowledge, and invite review of the findings themselves. 

### Summary of Findings

All findings are summarized in the Canon EF Protocol Reverse Engineering Summary document, currently at Draft 1. 

### Not Yet Ready Documents

I plan on uploading and sharing the various scripts, programs, and microcontroller firmware developed over the course of this project to allow others to use them for further work. The aim is to have all files documented and uploaded by the time the report reaches Version 1. 

Raw collected data, and processed versions of it will be uploaded for review and use as well. 


### Current State of The Project
At this time the EF protocol is understood to have at least 3 generations, each building on the previous and adding more features. Generation 1 is almost completely decoded with only a few remaining items to wrap up. Portions of Generation 2 are understood well enough to be used. Generation 3 is the least complete. 

### Planned Future Work
Based on initial investigation, it appears that the EF-m protocol is effectively just the Generation 3 EF protocol with very minor changes. Once Generation 3 has been fully decoded it should be possible to quickly verify the entirety of EF-m. 

I would like to repeat this work with the RF protocol in the future, but I am realistically a long way away. I've done some very basic data collection from RF cameras and there are both striking similarities and differences from EF. I strongly suspect that fully decoding Generation 3 of EF will provide a solid starting point for RF. 

## Repository structure

| Directory              | Content                                                                      |
| ---------------------- | ---------------------------------------------------------------------------- |
| [tools/](tools/)       | Assorted Scripts and Python Programs used to collect data and test theories. |
| [firmware/](firmware/) | RP2350 firmware for camera data collection                                   |
| [reports/](reports/)   | Reverse-engineering reports and methodology write-ups                        |
| [data/](data/)         | Raw and processed measurement data                                           |

## Contributing
I welcome any collaboration. Double-checking my methodology, flagging errors, or digging through the raw data for things I missed are all fair game.

- **Reports**: since these are PDFs and not easily diffable, please open an issue describing the error or finding rather than a PR. I'll fold it into the next draft with credit.
- **Tools / firmware**: PRs are welcome. For anything non-trivial, please open an issue first so we can agree on the approach before you put in the work.
- **Data**: if you've collected your own data and want to contribute it, open an issue or PR and I'll take a look.

By contributing, you agree your contribution is licensed under whichever license already applies to that part of the repo (see [Licensing](#licensing) below), and you'll be credited for it.



### Legal Stuff

This is an independent research project and is not affiliated with, endorsed by, or sponsored by Canon Inc. "Canon" and "EF" are trademarks of their respective owner. All findings here are the result of independent  observation and analysis of protocol behavior.
## Licensing

This repository is multi-licensed by content type — see [LICENSE](LICENSE)
for the full breakdown and [LICENSES/](LICENSES/) for the license texts:

- **Code** (`tools/`, `firmware/`): [Apache-2.0](LICENSES/Apache-2.0.txt)
- **Reports** (`reports/`): [CC-BY-SA-4.0](LICENSES/CC-BY-SA-4.0.txt)
- **Data** (`data/`): [CC0-1.0](LICENSES/CC0-1.0.txt)
