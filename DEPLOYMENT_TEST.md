# Deployment Test Notes

Source imported from:

- Repository: https://github.com/KegangWangCCNU/FacePhys-Demo
- Imported commit: `0eac651b0224e414a3da22e4b4629902378f7ca7`
- License: MIT License with Privacy Protection Addendum, see `LICENSE`

## Local Preview

Use a local HTTP server instead of opening `index.html` directly:

```bash
python3 -m http.server 8090
```

Then open:

```text
http://localhost:8090/
```

`localhost` is treated as a secure context by browsers, so webcam permission can be tested locally.

## GitHub Pages

Push these files to your GitHub repository root, then enable Pages from:

```text
Settings -> Pages -> Deploy from a branch -> main -> / (root)
```

Camera testing should be done on the final HTTPS Pages URL.

## Privacy Requirement

The upstream license requires local biometric processing by default. Do not add video or physiological-data upload logic unless users give explicit informed consent.
