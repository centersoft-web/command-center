# Command Center

O **Command Center** é uma central administrativa modular criada em HTML, CSS e JavaScript. O projeto reúne ferramentas financeiras, imobiliárias, patrimoniais e administrativas em uma interface única, com funcionamento local no navegador.

## Demonstração

Acesse a versão publicada:

**https://centersoft-web.github.io/command-center/**

## Sobre o projeto

A aplicação usa uma tela principal com navegação lateral e carrega os módulos em uma área central. O sistema foi desenvolvido para funcionar sem servidor próprio ou banco de dados externo, mantendo os dados no navegador do usuário.

## Funcionalidades

- Interface com tema corporativo escuro
- Navegação modular pela barra lateral
- Controle de acesso por senha
- Alteração ou remoção da senha
- Bloqueio manual da sessão
- Armazenamento local com `LocalStorage` e `IndexedDB`
- Backup completo em arquivo JSON
- Restauração completa dos dados
- Reset protegido de todos os dados locais
- Compatibilidade com instalação como aplicativo PWA
- Service worker para suporte à execução publicada

## Módulos disponíveis

| Módulo | Finalidade |
|---|---|
| Gestão de Aluguéis | Controle mensal de alugueis, pagamentos e dados de inquilinos |
| Imóveis, IPTU e Serviços | Administração patrimonial de imóveis |
| Gestão de Contratos | Organização de contratos |
| Gestão Financeira Global | Gestão financeira consolidada |
| Gestão de Contas Bancárias | Controle de contas bancárias |
| Gestão de Cartões de Crédito | Administração de cartões de crédito |
| Gestão de Cartões | Controle de parcelas e despesas |
| Quantum Trade | Gestão de operações financeiras e investimentos |
| FleetManager PRO | Controle de frota veicular |
| Agenda de Tarefas | Organização de atividades |
| Calculadoras e simuladores | Cálculos financeiros, trabalhistas e imobiliários |

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript puro
- LocalStorage
- IndexedDB
- Service Worker
- Web App Manifest
- Tailwind CSS por CDN
- Font Awesome por CDN
- Google Fonts

## Estrutura do projeto

```text
/
├── index.html
├── manifest.json
├── sw.js
├── icon.ico
├── icon-192.png
├── icon-512.png
├── Agenda de Tarefas.html
├── Calculadora Comparativa.html
├── Calculadora Financeira.html
├── Calculo Trabalhista.html
├── Controle de Reforma.html
├── FleetManager PRO.html
├── Gestão Cartões de Credito.html
├── Gestão Contas Bancárias.html
├── Gestão Financeira Global.html
├── Gestão de Aluguéis.html
├── Gestão de Contratos.html
├── Gestão de Cartões.html
├── Imóveis & IPTU & Serviços.html
├── Quantum Trade.html
├── Simulador IRPF – PF x PJ.html
├── Simulador de Custos Imobiliários.html
├── Simulador de Custos de Doação.html
└── README.md
```

## Como executar localmente

1. Baixe ou clone o repositório:

```bash
git clone https://github.com/centersoft-web/command-center.git
```

2. Entre na pasta:

```bash
cd command-center
```

3. Abra o arquivo `index.html` em um navegador moderno.

Mantenha todos os arquivos HTML na mesma pasta do `index.html`, pois os módulos são carregados por seus nomes de arquivo.

## Publicação no GitHub Pages

1. Abra o repositório no GitHub.
2. Acesse **Settings**.
3. Selecione **Pages**.
4. Em **Build and deployment**, escolha a branch `main`.
5. Selecione a pasta `/ (root)` e confirme.

A publicação em HTTPS é recomendada para utilizar corretamente o manifest, o service worker e a instalação como aplicativo.

## Armazenamento dos dados

Os dados são mantidos no navegador do usuário:

- `LocalStorage` para configurações e registros simples
- `IndexedDB` para dados estruturados dos módulos

Não há sincronização automática entre navegadores ou dispositivos.

## Backup e restauração

A área de configurações permite:

- Exportar todos os dados locais
- Restaurar um backup completo
- Criar um backup de segurança antes da restauração
- Apagar permanentemente os dados locais

Os backups podem ser usados para preservar os registros antes de trocar de navegador, limpar os dados do dispositivo ou reinstalar o aplicativo.

> A responsabilidade pelo backup é do usuário. Limpeza de cache, exclusão do perfil do navegador, formatação do computador ou remoção dos dados locais pode causar perda permanente das informações.

## Instalação como aplicativo

Em navegadores compatíveis, o projeto pode ser instalado pelo menu do navegador:

- Clique em **Instalar aplicativo** ou **Adicionar à tela inicial**.
- Confirme o nome e a instalação.
- Abra o aplicativo pelo menu Iniciar, área de trabalho ou tela inicial do dispositivo.

A instalação somente é garantida quando o projeto é publicado em HTTPS. Abrir apenas o `index.html` no computador não oferece o mesmo funcionamento de uma PWA.

## Requisitos

- JavaScript habilitado
- Suporte a LocalStorage e IndexedDB
- Navegador moderno
- Conexão com a internet para recursos carregados por CDN
- Publicação em HTTPS para instalação PWA completa

## Navegadores compatíveis

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Opera

## Observações

- O sistema não substitui autenticação ou armazenamento seguro em servidor.
- Os recursos visuais externos podem depender de conexão com a internet.
- Pop-ups e área de transferência podem exigir permissões do navegador.
- Os relatórios são preparados para impressão e geração de PDF pelo navegador.

## Aviso

Este projeto foi criado para uso administrativo e educacional de HTML, CSS e JavaScript. Os dados são armazenados localmente e podem ser perdidos caso o armazenamento do navegador seja removido.
