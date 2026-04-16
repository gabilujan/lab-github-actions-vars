# Respostas

## Por que a Secret aparece como ***?

Porque o GitHub protege automaticamente informações sensíveis, mascarando secrets nos logs para evitar vazamento de dados.

## O Job deploy_app consegue ler a variável BUILD_VERSION criada no Job build_app?

Não. Cada job roda em um ambiente isolado (runner diferente), então as variáveis não são compartilhadas automaticamente entre eles.