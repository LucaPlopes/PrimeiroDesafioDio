# Chaves SSH

Uma chave SSH te permite estabelecer uma conexão segura entre duas maquinas.

### Passos para criação

- Abrir o Git Bash
- Já dentro do terminal digitar o código
- ssh-keygen -t ed25519 -C + "adicionar o e-mail que você utiliza" (ENTER)
- O terminal pedirá sua senha (Digite + ENTER)
- Será criado um diretório contendo sua chave publica e privada criada --> /c/Users/"seu usuario"/ .ssh/
- Você irá caminhar até o repositório e digitará
- cat id_ed25519.pub "isso gerará um link no qual você irá colar no GitHub na Aba SSH Keys"
- Após isso iremos ativar a entidade que irá lidar com as chaves
- voltaremos ao terminal e digitaremos "eval $(ssh-agent -s)" e assim será criado o agente ou entidade
- depois entregaremos a chave privada para a entidade usando o comando "ssh-add id_ed25519"
- E prontinho sua chave está criada 🤲

