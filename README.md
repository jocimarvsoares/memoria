# Agenda & Memória IA

Aplicativo web offline em um único arquivo HTML.

## Funções
- Agenda mensal e eventos
- Diário: Filmes, Comida, Cotidiano, Trabalho, Hobbies/Experiências, Saúde e Outros
- Cadastro de pessoas e aniversários
- Lembretes de aniversário: 2 dias antes e no dia
- Perfil e preferências
- Campo Conceitos para registrar princípios, ideias e referências pessoais importantes
- Memórias consolidadas
- Backup/restauração em JSON
- Exportação de memória em CSV e TXT
- Dados persistidos no localStorage do navegador
- Funciona sem servidor

## Como usar
Abra `index.html` no Chrome/Edge/Firefox.

## Observação sobre notificações
Notificações do navegador dependem da permissão do usuário e, em um HTML local simples, não são garantidas quando o navegador estiver completamente fechado. Para notificações realmente confiáveis em segundo plano, transforme o projeto em PWA com Service Worker ou em aplicativo Android.

## Arquivo de memória
O botão "Baixar memória CSV" gera uma tabela estruturada para importação futura.
O "Baixar memória TXT" gera um contexto legível por outras IAs.
O backup JSON preserva todos os dados para restauração no próprio aplicativo.


## Cadastro de pessoas — ficha estruturada para IA
Cada pessoa possui uma ficha única com:
- nome
- relação
- aniversário
- nome do pai
- nome da mãe
- CPF
- telefone
- e-mail
- observações

Esses campos são preservados no backup JSON, exportados em colunas próprias no CSV e consolidados no TXT de memória virtual. Na camada de memória, a pessoa é representada como um objeto estruturado, para que uma IA consiga distinguir cada atributo e manter as relações entre os dados.

- Na página Pessoas, o cadastro é feito pelo botão “+ Cadastrar”, que abre uma janela com todos os campos da ficha. O cabeçalho da página fica fixo durante a navegação e ocupa menos espaço; a lista de registros permanece compacta. A edição continua sendo feita pela janela “Editar pessoa”.
