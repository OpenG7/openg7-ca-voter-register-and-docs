# OpenG7 — CA: Voter Register & Official Docs (openg7-ca-voter-register-and-docs)
**FR — OpenG7 — CA : Registre des électeurs & documents officiels (openg7-ca-voter-register-and-docs)**

> Ingest & normalize official updates; maintain a trustworthy voter register; generate and securely reprint official documents (printer gateway).
>
> Ingérer & normaliser les mises à jour officielles; maintenir un registre fiable; générer et réimprimer de façon sécurisée les documents officiels (passerelle imprimeur).

## Plain-language description / Description (grand public)
- **FR** — Il récupère les infos officielles (déménagements, décès), les met à jour proprement et produit la **première version de la liste des électeurs** ainsi que les **documents officiels**. S’il y a une erreur, on peut **corriger et réimprimer**. En bref : **on prépare tout avant le vote**.
- **EN** — It pulls official updates (moves, deaths), cleans them up and produces the **first version of the voter list** and the **official documents**. If there’s an error, we can **correct and reprint**. In short: **we prepare everything before voting**.

---
## Overview / Aperçu
- **OpenG7** public project. Code and configs here are **open-source**; production secrets and private endpoints live in a **separate private overlays repo**.
- **Contracts (schemas & APIs)** are defined in the *reference* repo: `openg7-electoral-systems-canada`.
- This service aims to be **transparent**, **auditable**, and **secure-by-default**.

## How to Run (dev) / Lancer en local (dev)
1. Install prerequisites: Docker or your preferred runtime.
2. Copy a sample config from `config/samples/` to `config/dev.yaml` and edit as needed.
3. Run the service:
   ```bash
   # Example placeholder. Replace with your real entrypoint later.
   python -m app.main --config config/dev.yaml
   ```
4. Run tests:
   ```bash
   pytest -q
   ```

## Security / Sécurité
- No personal data (PII) should be committed to this repo.
- Secrets are managed via environment variables or secret stores (Vault, cloud KMS), **never** in Git.
- See **SECURITY.md** for responsible disclosure and hardening tips.

## Contributing / Contribution
- Please read **CODE_OF_CONDUCT.md**.
- Open issues/PRs in English or French.
- Keep changes backward-compatible with published **contracts** when possible.

## License / Licence
- Code: MIT © 2025 OpenG7 contributors.
