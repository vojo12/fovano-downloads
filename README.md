# Fovano — distribuição

Canal público de download do Fovano para Windows. Contém a página estática de distribuição; o código do aplicativo permanece no projeto privado local.

- `index.html`: página de download, sem dependências ou build.
- `vercel.json`: redireciona `/download` ao instalador publicado nas Releases.
- `Fovano-Setup-0.1.0.exe.sha256`: integridade do instalador.

O instalador é um asset da Release `v0.1.0`, fora do histórico Git por exceder o limite de 100 MiB por arquivo. A Vercel está conectada à branch `main`; futuros pushes publicam a página automaticamente.

Para publicar outra versão, envie o novo instalador e checksum a uma Release, atualize o redirecionamento e os dados da página e faça push para `main`.
