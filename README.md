# pi-discovery

O `pi-discovery` é um pacote de distribuição focado em **Product Discovery**, **Engenharia de Requisitos** e **Especificação de Projetos**. Ele injeta inteligência de negócios no [Pipa Core](https://github.com/aelinrezende/pipa), transformando a orquestradora genérica em um verdadeiro esquadrão ágil de produto.

Ao invés de programar código-fonte, este pacote é focado em transformar *briefings* caóticos e ideações em especificações técnicas precisas, arquitetura de software, fluxos de UX e backlogs estruturados.

## 📦 Instalação

Adicione o pacote nas configurações do seu Pi (`settings.json` ou `package.json`):

```json
"packages": [
  "git:github.com/pipalabs/pi-discovery"
]
```

## 🚀 Como Funciona

Ao ser carregado, a arquitetura base da Pipa (Pipa Core) detecta este pacote e configura o ambiente local (`.pi/`) com as regras de domínio exclusivas para a área de Produto, trazendo um "Squad Hiper-Especializado" completo.

### 👑 A Orquestradora (Pipa)
A Pipa é a orquestradora do Discovery: recebe os *briefs* iniciais, invoca os colegas do squad, coordena o fluxo e valida as entregas finais antes de devolvê-las. Pipa não faz o trabalho braçal — ela delega.

### 🤝 O Squad de Discovery (Teammates)
Para extrair a especificação perfeita, o squad conta com:

1. **Barbara (Product Manager):** A líder estratégica do Discovery. Define o escopo geral, coordena o time de especificação e valida as entregas finais.
2. **Isa (Product Owner):** A tradutora do negócio. Ela pega o brief da Barbara e escreve as **regras de negócio** detalhadas, descrevendo atores, fluxos e condições sem ambiguidade.
3. **Hugo (Arquiteto de Soluções):** O designer do sistema. Baseado nas regras da Isa, ele mapeia a **arquitetura**, definindo módulos, endpoints de API e contratos de dados (DTOs).
4. **Pamela (UX Designer):** A defensora do usuário. Ela mapeia as jornadas e descobre as **interfaces implícitas** (ex: telas de erro, confirmações e fluxos que não estavam explícitos nas regras).
5. **Stephanie (Tech Lead):** A avaliadora de risco. Ela lê a arquitetura definida pelo Hugo e elabora uma análise de **complexidade técnica**, apontando riscos e sugerindo a alocação ideal de desenvolvedores.
6. **Gabriel (Agile Master):** O organizador. Ele pega tudo o que foi validado e quebra em tarefas atômicas, estruturando um **backlog final (CSV)** com estimativas de tempo e dependências prontas para a *sprint*.

## 🛠️ Utilização Prática

1. Inicie a sessão passando o briefing cru do cliente para a **Barbara**.
2. A Barbara irá invocar a **Isa** para detalhar as regras de negócio.
3. Com as regras prontas, ela coordenará o trabalho entre **Pamela**, **Hugo** e **Stephanie** para mapear UX, Arquitetura e Complexidade.
4. Por fim, o **Gabriel** será acionado para tabular o esforço em um backlog.
5. A Barbara faz a revisão final e te entrega os artefatos prontos (Regras, Arquitetura, UX, Backlog e Análise de Risco) na pasta `.pi/artifacts/`.
