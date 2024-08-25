# kt-sdvx-eamuse-importer

Import your scores from https://p.eagate.573.jp/game/sdvx/vi to [Kamaitachi](https://kamai.tachi.ac/).

This aims to be the successor to Kamaitachi's "E-Amusement CSV" import method, as this method includes data for timestamps, judgements, max combo, and EX score.

# Installation / Usage

1. Install [Python 3.9](https://www.python.org/downloads/) or newer.
2. Clone this repository or [download from Releases](https://github.com/tranq88/kt-sdvx-eamuse-importer/releases/latest).
3. Open a terminal in the main directory and install the dependencies with `pip install -r requirements.txt`.
4. Go [here](https://kamai.tachi.ac/client-file-flow/CIab02b801e1519f4be46c7d4f095147298ad84d64) to download a `config.ini` containing your API key. Don't share this key with anyone!
5. Put `config.ini` next to `main.py` and fill out the `username` and `password` fields with your KONAMI / e-amusement credentials.
6. Run the program with `python main.py`.

# Notes

- KONAMI doesn't return accurate CRITICAL judgement data, so it's simply not sent to Kamaitachi.
