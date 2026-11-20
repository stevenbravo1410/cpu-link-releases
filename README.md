# CPU Link — tester releases

Windows x64 distributions for CPU Link, a local MCP server for Lighter from CPU Protocol
(Capital Processing Unit). This repository contains release packages and the signed tester
update feed. The development repository remains private during testing.

**This repository is public. Anyone can access these files.** It is not a password-protected
tester portal. Use a dedicated low-balance test account; never upload credentials or private reports.

## Install and update

Download the Windows desktop + CLI or CLI-only ZIP from **Releases**, extract it completely,
and follow `LEEME-README.html`. Python and dependencies are included. Alpha9 introduces the
updater and requires one manual installation. From then on, open **Updates → Check for updates**.

There is one channel: **testers**. Checks are manual by default; optional six-hour checks run
while the GUI is open. Installation always requires your action. CPU Link verifies an Ed25519
signature plus the package SHA-256, preserves local settings/credentials, keeps a backup and
restarts its own service. Reconnect your AI client afterwards. No AI applications are force-killed.

No account data, keys, trades, usage analytics or reports are uploaded. GitHub receives ordinary
network requests (including IP information) and may count downloads. The manifest signature is
not Windows Authenticode signing or a third-party security audit.

The public update feed is `testers/windows-amd64.json`. It has a signed payload and signature;
the verification key pinned in the application is:

```
15fd8053884bc8f780832f20aab86afd04ea94417ade093e1bf9772453581eb0
```

## Español

Descarga el ZIP de Windows en **Releases**, extráelo por completo y abre `LEEME-README.html`.
Alpha9 se instala manualmente una vez; después puedes buscar actualizaciones desde CPU Link.
Solo existe el canal de testers. Las búsquedas periódicas son opcionales y la instalación
siempre requiere tu acción. Reconecta tu IA cuando termine.

La configuración y las credenciales se conservan localmente. No se envían operaciones ni
reportes automáticamente. Este repositorio es público y GitHub puede ver la IP de las solicitudes.
Nunca compartas claves API ni claves de tu wallet.
