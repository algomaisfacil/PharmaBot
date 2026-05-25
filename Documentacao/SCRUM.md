# SCRUM

Este documento apresenta a estrutura, o planejamento e a simulação da gestão ágil aplicada ao desenvolvimento do projeto **PharmaBot**, atendendo aos requisitos de Curricularização da Extensão da FATEC Campinas.

---

## Papéis do Scrum (Scrum Team)

* **Product Owner (PO):** Alexandre Watanabe Stefen  
  *(Responsável pela ponte direta com o proprietário/gestor da farmácia parceira, levantamento de necessidades reais do estabelecimento e priorização do Backlog de acordo com o negócio).*
* **Scrum Master:** Mario Celso Feitosa Ferreira  
  *(Responsável pela organização do fluxo de trabalho, garantia dos prazos acadêmicos, remoção de impedimentos de ferramentas e estruturação da documentação).*
* **Equipe de Desenvolvimento (Developers):** Alexandre Watanabe Stefen e Mario Celso Feitosa Ferreira  
  *(Ambos atuam em conjunto na modelagem de requisitos, escrita das narrativas, especificação do plano de testes e prototipagem no Figma).*

---

## Product Backlog Geral
Mapeado diretamente a partir das necessidades levantadas para a comunidade (clientes da farmácia) e traduzidas no **Diagrama de Casos de Uso**:

### Módulo 1: Engenharia de Requisitos e Modelagem (Fase Atual)
* **PB01:** Levantamento de requisitos e criação do Diagrama de Casos de Uso.
* **PB02:** Elaboração das narrativas detalhadas dos Casos de Uso.
* **PB03:** Criação do protótipo de telas de alta fidelidade no Figma.
* **PB04:** Elaboração do Plano de Testes de Software.

### Módulo 2: Informações e Atendimento Automatizado (Bot)
* **PB05:** Desenvolver caso de uso *Informações Loja* (Endereço, horários, telefones úteis).
* **PB06:** Desenvolver caso de uso *Disponibilidade Medicamento* (Consulta automatizada de estoque).

### Módulo 3: Transbordo (Atendimento Humano)
* **PB07:** Desenvolver caso de uso *Conversar Funcionário* (Lógica para pausar o bot e acionar a fila humana).
* **PB08:** Desenvolver fluxo de resposta *Conversar com cliente* para a interface do ator Farmacêutico.

### Módulo 4: Agendamentos e Disparos Automáticos
* **PB09:** Desenvolver caso de uso *Agendar Horário Medicamento*.
* **PB10:** Desenvolver caso de uso *Ver agendamentos* ativos do cliente.
* **PB11:** Desenvolver caso de uso *Modificar Horário* cadastrado.
* **PB12:** Desenvolver rotina em segundo plano para o disparo do caso de uso *Enviar Lembretes*.

---

## Planejamento da Sprint

* **Duração:** 14 dias (Duas semanas - Foco exclusivo em Modelagem e Engenharia de Software)
* **Data de Início:** 13/05/2026
* **Data de Término:** 27/05/2026
* **Meta da Sprint:** Entregar toda a especificação técnica, prototipagem, plano de testes e estrutura de configuração do PharmaBot validada.

### Sprint Backlog (Tarefas Selecionadas)

| ID | Tarefa | Esforço Estimado (Horas) | Responsável | Status |
| :--- | :--- | :---: | :--- | :---: |
| TS01 | Refinar o Diagrama de Casos de Uso e escrever as narrativas | 10h | Equipe | **Concluído** |
| TS02 | Criar proposta de Interface no Figma baseada nas Heurísticas de Nielsen | 15h | Equipe | **Concluído** |
| TS03 | Configurar Repositório no GitHub e aplicar as regras de GCS (AndersonLuizBarbosa) | 3h | Scrum Master | **Concluído** |
| TS04 | Elaborar o Plano de Testes (Tabela de Cenários) e documentar o SCRUM | 12h | Equipe | **Concluído** |

**Total de Esforço Planejado:** 40 horas.

---

## Execução da Sprint e Gráfico de Burndown

Para medir a eficiência e a queima de esforço diário do grupo, coletamos os dados da evolução do trabalho em horas restantes:

### Tabela de Evolução da Sprint (Acompanhamento Diário)

| Dia da Sprint | Data | Trabalho Restante Ideal | Trabalho Restante Real | Evento / Justificativa |
| :---: | :---: | :---: | :---: | :--- |
| Dia 1 | 13/mai | 40h | **40h** | Reunião de Planejamento da Sprint realizada com sucesso. |
| Dia 3 | 15/mai | 34h | **38h** | TS03 concluída. Repositório e acessos configurados. |
| Dia 6 | 18/mai | 25h | **28h** | Diagrama de Casos de Uso fechado e início das narrativas. |
| Dia 8 | 20/mai | 20h | **20h** | TS01 concluída. Narrativas documentadas na pasta principal. |
| Dia 10 | 22/mai | 14h | **18h** | Pequeno atraso na vetorização dos componentes do WhatsApp no Figma. |
| Dia 12 | 24/mai | 6h | **5h** | TS02 concluída. Protótipo de alta fidelidade finalizado no Figma. |
| Dia 14 | 25/mai | 0h | **0h** | TS04 concluída. Plano de testes fechado e documentação pronta para entrega. |