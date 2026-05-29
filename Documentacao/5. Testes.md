# Plano e Casos de Teste

Este documento apresenta o plano de testes e os cenários simulados para garantir a qualidade e a aderência aos requisitos do sistema **PharmaBot**, conforme solicitado na Etapa 5 do projeto de extensão.

---

## Metodologia de Teste
Como o sistema ainda está em fase de modelagem, aplicamos a técnica de **Teste de Caixa Preta** baseada nos Casos de Uso mapeados. Os testes validam as entradas do usuário (mensagens no WhatsApp) e os resultados esperados gerados pelo bot ou pelo transbordo humano.

---

## Casos de Teste

| ID | Caso de Uso Relacionado | Cenário de Teste | Entrada (Input) | Resultado Esperado |
| :---: | :--- | :--- | :--- | :--- |
| **CT01** | Menu Inicial / Saudação | Cliente inicia o contato com a farmácia | Mensagem: "Olá, gostaria de ajuda." | O PharmaBot deve responder instantaneamente enviando a saudação padrão e o Menu Principal de opções. |
| **CT02** | Informações Loja | Cliente deseja saber o horário de funcionamento | Digitar a opção correspondente a "Informações Loja" (ex: "1") | O sistema deve exibir o endereço completo, telefone de contato e os horários de abertura/fechamento da farmácia. |
| **CT03** | Disponibilidade Medicamento | Cliente consulta um medicamento em estoque | Digitar a opção "Disponibilidade" e enviar "Dipirona 500mg" | O sistema deve simular a busca e retornar se o medicamento está disponível e o valor aproximado. |
| **CT04** | Conversar Funcionário / Cliente | Cliente solicita falar com um atendente humano | Digitar a opção "Falar com Atendente" (ex: "3") | O PharmaBot deve enviar uma mensagem informando que está transferindo o atendimento e notificar o ator **Farmacêutico**. |
| **CT05** | Agendar Horário Medicamento | Cliente cadastra um novo lembrete | Selecionar "Agendar Horário" -> Enviar "Paracetamol às 20:00" | O sistema deve confirmar o agendamento: "Lembrete para Paracetamol cadastrado às 20:00 com sucesso". |
| **CT06** | Ver agendamentos | Cliente consulta seus alarmes ativos | Selecionar a opção "Ver agendamentos" | O bot deve listar todos os medicamentos e horários salvos para aquele número de WhatsApp. |
| **CT07** | Modificar Horário | Cliente altera um agendamento existente | Selecionar "Modificar Horário" -> Escolher o alarme -> Enviar novo horário ("22:00") | O bot deve atualizar o registro e confirmar a alteração para as 22:00. |
| **CT08** | Enviar Lembretes | Disparo automático do lembrete no horário configurado | O relógio do sistema atinge o horário agendado (ex: 20:00) | O sistema deve disparar de forma ativa a mensagem na conversa do cliente: "Está na hora de tomar o seu Paracetamol!". |

---

## Tratamento de Erros

Também foram mapeados cenários onde o usuário interage de forma inesperada, garantindo a robustez do bot (Heurísticas de Nielsen - Prevenção de Erros):

| ID | Cenário de Erro | Entrada (Input) | Resultado Esperado |
| :---: | :--- | :--- | :--- |
| **CT09** | Entrada de opção inválida no menu | Usuário envia uma opção que não existe (ex: "9" ou "Texto aleatório") | O PharmaBot deve responder com uma mensagem amigável informando que não entendeu, e reenviar o Menu Principal de forma limpa. |
| **CT10** | Medicamento Não Encontrado | Usuário busca por um produto que a farmácia não trabalha | Enviar nome de um produto inexistente na busca de estoque | O bot deve informar que o produto não foi localizado e oferecer a opção de transferir para o atendente humano. |
