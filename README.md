# retro-anki-sync-server

**retro-anki-sync-server** is a fork of 
[tsudoko/anki-sync-server](https://github/https://github.com/tsudoko/anki-sync-server)

As the purpose of this fork is just for me to try things out: I strongly 
recommend that you do **not**, under any circumstances, attempt to use this as 
your anki-sync-server.  If you are looking for an anki-sync-server to use please 
be aware that Anki now includes a 
[build in sync-server](https://docs.ankiweb.net/sync-server.html)

## Setup

- `git clone https://github.com/peterclifton/retro-anki-sync-server.git`
- Setup a python virtual environment
    - `python -m venv retro-anki-sync-venv`
    - `source retro-anki-sync-venv/bin/activate`
    - `pip install --upgrade pip`
    - `pip install -r retro-anki-sync-server/anki-bundled/requirements.txt`
    - `pip install webob`

## Launching the server

- Activate the python virtual environment (if not already activated):
    - `source retro-anki-sync-venv/bin/activiate`
- Make sure *anki* and *ankisyncd* are in the python path
    - `cd retro-anki-sync-server`
    - `PYTHONPATH="$PYHONPATH:$PWD:$PWD/anki-bundled`
    - `export PYTHONPATH`
- `python ankisyncd/sync_app.py ankisyncd.conf`

---

## The original README

The README from 
[tsudoko/anki-sync-server](https://github/https://github.com/tsudoko/anki-sync-server)
as it was at the time **retro-anki-sync-server** was forked from 
[tsudoko/anki-sync-server](https://github/https://github.com/tsudoko/anki-sync-server)
is provided [here](docs/Appendix.md) for reference.

