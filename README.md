# Miroirs MinIO

Conservation des images communautaires officielles MinIO retirées des registres
publics utilisés précédemment. Les images sont republiées sans reconstruction,
uniquement pour `linux/amd64`.

| Image | Version | Source |
| --- | --- | --- |
| `ghcr.io/humans-connexion/minio` | `RELEASE.2025-09-07T16-13-09Z` | [MinIO, commit 07c3a429](https://github.com/minio/minio/tree/07c3a429bfed433e49018cb0f78a52145d4bedeb) |
| `ghcr.io/humans-connexion/minio-client` | `RELEASE.2025-08-13T08-35-41Z` | [mc, commit 7394ce0d](https://github.com/minio/mc/tree/7394ce0dd2a80935aded936b09fa12cbb3cb8096) |

Les archives Docker, leurs empreintes SHA-256 et les métadonnées des images sources
sont conservées dans la release `upstream-2026-09-24`. Les binaires MinIO et mc
conservent leur licence GNU AGPLv3 et leurs mentions d'origine ; les composants
de l'image conservent leurs propres licences.

Le workflow manuel **Publier les miroirs MinIO** vérifie les empreintes des archives,
charge les images, puis publie les deux packages avec le jeton GitHub Actions du
dépôt. Aucun secret personnel n'est nécessaire au workflow. Les packages doivent
être publics pour permettre les téléchargements anonymes.

Les consommateurs doivent épingler les digests publiés, en complément des tags
de version. Le miroir ne fournit aucune mise à jour de sécurité automatique.
La décision de remplacement de MinIO est à réexaminer au plus tard le
**24 octobre 2026**.
