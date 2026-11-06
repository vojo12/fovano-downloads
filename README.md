# Fovano — site e distribuição

Site público do Fovano (https://fovano-downloads.vercel.app) e canal de download para Windows. As páginas são geradas
pelo projeto do aplicativo (`site/build.mjs`); o código do aplicativo permanece no projeto privado.

- `index.html`, `baixar.html`, `funcoes/`, `custos.html`, `privacidade.html`, `novidades.html`, `ajuda.html`: páginas estáticas, sem JavaScript.
- `vercel.json`: endereços limpos, `/download` para o instalador da Release atual e a política de segurança.
- `Fovano-Setup-0.2.0.exe.sha256`: integridade do instalador da versão atual (as anteriores ficam para conferência).

Os instaladores ficam nos assets das Releases, fora do histórico Git, por excederem o limite de 100 MiB por arquivo.
A Vercel está conectada à branch `main`: cada push publica o site.
