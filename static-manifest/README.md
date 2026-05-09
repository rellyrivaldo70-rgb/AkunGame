# Example Static Hosting Bundle

Folder ini sudah berisi bundle contoh yang bisa kamu upload ke hosting publik:

- `modlist.json`
- `version.json`
- `files/skin/cj-streetwear-skin.zip`
- `files/vehicle/elegy-retro-pack.zip`

Kalau kamu mau langsung cocok dengan workflow GitHub Release default, copy isi folder ini ke:

```text
static-manifest/
```

Catatan penting:

- Kedua file zip di atas adalah `template demo`, bukan asset mod GTA final.
- Isinya placeholder yang aman untuk contoh struktur NETRALHUB.
- Kalau mau dipakai production, ganti isi zip dengan mod milikmu sendiri lalu generate ulang manifest.

Manifest URL contoh setelah diupload:

```text
https://domainkamu.com/netralhub/netral-rp/modlist.json
```

Kalau memakai `GitHub Releases`, URL manifest-nya akan berbentuk:

```text
https://github.com/OWNER/REPO/releases/download/static-manifest/modlist.json
```

Workflow otomatis untuk publish ke GitHub sudah disiapkan di:

```text
.github/workflows/publish-static-manifest.yml
```

Repo harus `public` kalau URL ini mau dipakai player lain tanpa login GitHub.

Di aplikasi NETRALHUB, kamu juga bisa isi:

- `GitHub Repo`: `OWNER/REPO`
- `Release Tag`: `static-manifest`

dan biarkan `Manifest URL` kosong. Client akan membentuk URL GitHub Release otomatis.
