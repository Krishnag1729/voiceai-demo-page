# VoiceAI demo page

GitHub Pages landing page for the VoiceAI offline English → Hindi voice translator.

The translator itself runs on a personal machine (source stays in the private `VoiceAI` repo) and is
exposed through a Gradio share tunnel while that machine is up. This page just reads `live.json` and
points at whatever tunnel URL is current, so the link in a syllabus/submission form never has to change.

To refresh the live URL: run `scripts/go_live.sh` in the `VoiceAI` repo on the host machine — it starts
the app with `--share`, updates `live.json` here, and pushes.
