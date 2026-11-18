EMPRESTIMO DIARIO - PROJETO ANDROID COM COMPILACAO AUTOMATICA

O aplicativo abre o sistema em:
https://emprestimo-diario-7ab01ded.base44.app/login

DADOS DO APP
- Nome: Emprestimo Diario
- Identificador: br.com.xistech.emprestimodiario
- Versao: 1.0
- Plataforma: Android (WebView)

COMO GERAR O APK PELO GITHUB (SEM ANDROID STUDIO)
1. Baixe e extraia este ZIP.
2. Entre em https://github.com e crie um repositorio novo (pode ser privado).
3. Envie todos os arquivos e pastas deste projeto para a raiz do repositorio. IMPORTANTE: envie tambem a pasta oculta .github/workflows.
   - Pelo site do GitHub: Add file > Upload files; arraste os arquivos e pastas extraidos.
   - Ou use GitHub Desktop para publicar a pasta do projeto.
4. No repositorio, abra a aba Actions.
5. Se solicitado, habilite GitHub Actions.
6. Selecione "Compilar APK Android" e clique em "Run workflow". Um envio para main/master tambem inicia a compilacao automaticamente.
7. Aguarde o workflow ficar verde. Abra a execucao concluida e baixe o artefato "EmprestimoDiario-APK" na secao Artifacts.
8. Extraia o ZIP do artefato. Dentro dele estara o arquivo app-debug.apk. Transfira-o para o Android e instale.

REQUISITOS E OBSERVACOES
- A compilacao usa GitHub Actions, Java 17, Gradle 8.9 e Android SDK 35.
- O APK gerado e de depuracao (debug), adequado para testes e instalacao manual. Para publicar na Play Store, sera necessario configurar assinatura de release.
- O app requer internet e usa HTTPS. Login, cookies e autenticacao externa dependem do funcionamento e das politicas da plataforma Base44.
- Nao compartilhe credenciais de acesso ao GitHub. O projeto nao contem senhas nem chaves de assinatura.
