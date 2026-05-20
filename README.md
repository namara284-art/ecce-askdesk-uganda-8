# ECCE AskDesk Uganda — Logo-Embedded Render Build

This build fixes missing logo issues on Render.

What changed:
- The MoES logo is embedded directly into `frontend/index.html`.
- The theme logo is embedded directly into `frontend/index.html`.
- The embedded homepage inside `app.py` is also updated with the embedded logos.
- This avoids broken image paths on Render.

## Render settings

Build Command:

```bash
python -m pip install --upgrade pip setuptools wheel && pip install -r requirements.txt
```

Start Command:

```bash
python -m uvicorn app:app --host 0.0.0.0 --port $PORT
```

Pre-deploy Command: leave empty.

Root Directory: leave empty.
