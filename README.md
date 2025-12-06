# API Documentation Project

## 📂 Latest Documentation
The `docs/` folder contains the most up-to-date API documentation:

- [Login](docs/Login.md)
- [Profile](docs/Profile.md)
- [Orders](docs/Orders.md)
- [Logout](docs/Logout.md)
- [Payments](docs/Payments.md)
- [Settings](docs/Settings.md)

---

## 🔖 Version Snapshots
Frozen snapshots of documentation are stored in the `versions/` folder:

- [v1.0](versions/v1.0/) → Login, Profile
- [v1.1](versions/v1.1/) → + Orders, Logout
- [v1.2](versions/v1.2/) → + Payments, Settings

Each snapshot is tagged in Git for traceability:
- `doc-v1.0`
- `doc-v1.1`
- `doc-v1.2`

---

## 📢 Release Notes
Detailed release notes are available in the `release-notes/` folder:

- [v1.0](release-notes/v1.0.md) – Initial release (Login, Profile)
- [v1.1](release-notes/v1.1.md) – Added Orders & Logout
- [v1.2](release-notes/v1.2.md) – Added Payments & Settings, updated Profile

---

## ✅ Workflow
1. Add or update API docs in `docs/`.
2. Copy all docs into a new snapshot folder under `versions/vX.Y/`.
3. Stage and commit changes:
   ```bash
   git add docs/* versions/vX.Y/
   git commit -m "Update docs; snapshot vX.Y"
   git tag doc-vX.Y
   git push origin main --tags