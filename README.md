# appsec-lab

Web vulnerability classes, written from scratch: for each class, a tiny Flask route with the flaw, a test that exploits it, and the fixed route.

> **Intentionally vulnerable code. Run it locally only. Never expose it to a network.**

## Progress

| Class | Academy topic | Note | Vulnerable route | Exploit test | Fixed route | Cold redo |
| --- | --- | --- | --- | --- | --- | --- |
| SQL injection | [link](https://portswigger.net/web-security/sql-injection) | [ ] | [ ] | [ ] | [ ] | |
| IDOR (access control) | [link](https://portswigger.net/web-security/access-control/idor) | [ ] | [ ] | [ ] | [ ] | |
| Path traversal | [link](https://portswigger.net/web-security/file-path-traversal) | [ ] | [ ] | [ ] | [ ] | |

Add a row when you start a new class. Tick a box only when the file is committed.

## How each class is organized

- `notes/<class>.md`: the five-line note, a source-to-sink trace, and a 90-second explanation, all in your own words
- `classes/<class>/vulnerable.py`: a 10 to 15 line Flask route with the exact flaw
- `classes/<class>/fixed.py`: the same route, fixed
- `classes/<class>/test_<class>.py`: an exploit test that fails against `vulnerable.py` and passes against `fixed.py`

## Run it

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
pytest
```

## How this was built

The folder structure and this README were AI-assisted. The vulnerable routes, fixes, and tests are written by me, and every exploit was run by me on localhost. Update this section if that changes.

## Rules

- Local only, labeled intentionally vulnerable.
- No pasted lab text or step-by-step lab solutions. Link to the Academy topic instead.
- One commit per class.
