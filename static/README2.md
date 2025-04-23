🚀 Crypto Ecosystems v1.2 Update [2024]
A nova versão da taxonomia do Crypto Ecosystems já está disponível! Confira os detalhes da atualização neste link.

🌐 Crypto Ecosystems
Licença MIT com atribuição

Crypto Ecosystems é uma taxonomia colaborativa voltada para dados de ecossistemas de blockchain, Web3, criptomoedas e projetos descentralizados. Ela conecta esses dados a organizações e repositórios do GitHub, estruturados em arquivos de configuração no formato TOML.

Este repositório está em constante evolução — e isso é intencional! Novos projetos surgem todos os dias, e nosso objetivo é acompanhar esse crescimento.

🤝 Como Contribuir
Existem duas formas principais de contribuir com o projeto:

✅ Opção 1: Abrindo um Pull Request
Você pode:

Criar um novo arquivo .toml para um ecossistema na pasta /data/ecosystems, ou

Editar um arquivo existente para melhorar as informações.

Abra um PR a partir do seu fork. Se não souber como, assista este vídeo tutorial.

🗂️ Exemplo de Formato de Dados
toml
Copiar
Editar
title = "Bitcoin"
sub_ecosystems = ["Lightning", "RSK Smart Bitcoin", "ZeroNet"]
github_organizations = [
  "https://github.com/bitcoin",
  "https://github.com/bitcoin-core",
  "https://github.com/bitcoinj"
]

[[repo]]
url = "https://github.com/bitcoin/bitcoin"
tags = ["Protocol"]

[[repo]]
url = "https://github.com/bitcoinbook/bitcoinbook"
tags = ["Documentation"]
✍️ Opção 2: Usar o Formulário de Submissão
Não é dev? Sem problemas! Preencha o formulário no Airtable e nós cuidamos do resto.

📢 Como Fazer Atribuição
Para utilizar o Crypto Ecosystems Mapping da Electric Capital, a atribuição é obrigatória:

Elementos obrigatórios:

Fonte: “Electric Capital Crypto Ecosystems Mapping”

Link: https://github.com/electric-capital/crypto-ecosystems

Logo: Electric Capital logo

Recomendado: Incentivar outras pessoas a contribuírem:

"Se você trabalha com código aberto em cripto, envie seu repositório para ser contado!"

Exemplo de atribuição:

Fonte dos dados: Electric Capital Crypto Ecosystems Mapping
Se você trabalha com cripto open source, envie seu repositório aqui!

🧭 Guia de Contribuição — Passo a Passo
Você pode contribuir de três maneiras:

Adicionar um novo ecossistema (ex: uma blockchain L1)

Adicionar um sub-ecossistema (ex: um projeto dentro de um ecossistema maior)

Adicionar um repositório ou organização GitHub

Cada contribuição segue um caminho diferente — veja abaixo o guia completo para cada tipo:

🌱 1. Novo Ecossistema (L1)
Exemplo: adicionar a blockchain fictícia "EasyA Chain"

Navegue até /data/ecosystems

Crie o arquivo easya-chain.toml em /data/ecosystems/e/

Estrutura básica:

toml
Copiar
Editar
title = "EasyA Chain"
github_organizations = ["https://github.com/EasyA-Tech"]
Importante: não é necessário listar todos os repositórios da organização, eles são puxados automaticamente.

🌿 2. Novo Sub-ecossistema
Exemplo: adicionar “EasyA Community Wallet” como parte da "EasyA Chain"

Edite easya-chain.toml para adicionar:

toml
Copiar
Editar
sub_ecosystems = ["EasyA Community Wallet"]
Crie easya-community-wallet.toml em /data/ecosystems/e/ com:

toml
Copiar
Editar
title = "EasyA Community Wallet"
github_organizations = ["https://github.com/EasyA-Community-Wallet"]
📁 3. Novo Repositório ou Organização
Organização:
Adicione a URL da nova organização no campo github_organizations.

Repositório isolado:
Adicione ao final do .toml correspondente:

toml
Copiar
Editar
[[repo]]
url = "https://github.com/platonicsocrates/easya-helpers"
tags = ["Library"] # Opcional
❤️ Obrigado por contribuir!
Sua ajuda fortalece toda a comunidade de código aberto em cripto. Se tiver dúvidas, estamos por aqui para ajudar!
