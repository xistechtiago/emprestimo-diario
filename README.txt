EMPRESTIMO DIARIO - PROJETO ANDROID COM GITHUB ACTIONS

O projeto compila o aplicativo Android que abre:
https://emprestimo-diario-7ab01ded.base44.app/login

COMO PUBLICAR
1. Extraia o ZIP.
2. Crie um repositorio no GitHub chamado emprestimo-diario.
3. Envie o CONTEUDO da pasta EmprestimoDiarioAndroid para a raiz do repositorio, incluindo a pasta oculta .github.
4. Abra a aba Actions no repositorio.
5. Selecione "Compilar APK Android" e clique em "Run workflow".
6. Aguarde o job terminar com sucesso.
7. Na pagina da execucao, em Artifacts, baixe EmprestimoDiario-APK.
8. Extraia o arquivo baixado para obter app-debug.apk.

COMPILACAO AUTOMATICA
O workflow usa o Android SDK preinstalado no runner ubuntu-latest, verifica/instala a plataforma Android 35 e Build Tools 35.0.0, configura Java 17 e Gradle 8.9 e publica o APK como Artifact por 14 dias.

DADOS DO APP
Nome: Empréstimo Diário
Application ID: br.com.xistech.emprestimodiario
Versão: 1.0

OBSERVAÇÃO
Este pacote contém o código-fonte e a automação de compilação. O APK só será criado após executar o workflow no GitHub. Se o workflow ainda falhar, envie o log completo da etapa que falhou.
