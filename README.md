# Modmail — Privacy-focused (clean) fork

This repository is a cleaned, privacy-focused fork of Modmail intended for self-hosted use. It does not perform automatic telemetry or metadata uploads to external servers.

Summary

- Purpose: A simple, self-hosted Modmail instance for Discord servers.
- Privacy: Automatic metadata uploads and telemetry have been removed or disabled.

Privacy & Security

- This fork disables automatic external data transmission (for example, to `api.modmail.dev`).
- External uploads/hosts (Imgur, Hastebin) are disabled; the plugin registry is loaded from the local `plugins/registry.json` when available.
- Check `core/config.py` for the `data_collection` setting and set it to `False` for extra assurance.

What was removed or disabled

- Periodic metadata uploads to the Modmail API
- Automatic autoupdate startup
- External image and log uploads (Imgur, Hastebin)
- Remote plugin registry fetch (uses local `plugins/registry.json` if present)

Notes

- This README is intentionally concise. The original project contains more extensive documentation, but this fork prioritizes privacy by removing automatic telemetry and external uploads.

Clean Fork
