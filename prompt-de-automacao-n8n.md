# creative-challenge

Atue como um especialista em N8N.
Crie uma automação para classificar e responder automaticamente tickets de suporte recebidos por e-mail.

Público:
Equipe de atendimento ao cliente e suporte técnico.

Ferramentas envolvidas:
Gmail (ou IMAP/SMTP), OpenAI (ou Gemini API), Google Sheets e Slack (ou Discord).

Fluxo:
1. Monitorar a caixa de e-mails de suporte e capturar novas mensagens recebidas.
2. Enviar o título e corpo do e-mail para o modelo de IA classificar a urgência (Alta, Média, Baixa) e a categoria (Financeiro, Técnico, Dúvida Geral, Elogio/Feedback).
3. Gerar uma proposta de resposta inicial personalizada e profissional utilizando a IA.
4. Caso a prioridade seja Alta (Bug Crítico/Reclamação Urgente), enviar uma notificação imediata em um canal do Slack/Discord para a equipe humana assumir o atendimento.
5. Salvar o registro do ticket com dados do cliente, classificação e status em uma planilha do Google Sheets.
6. Enviar a resposta automática de confirmação ou solução para o e-mail do cliente.

Regras:
- Ignorar e-mails automáticos, noreply, newsletters ou mensagens marcadas como spam.
- E-mails de alta prioridade devem obrigatoriamente notificar a equipe humana antes de qualquer fechamento.
- A resposta gerada deve ser cortês, clara e estruturada em formato JSON válido para processamento seguro no N8N.

Explique quais nós do N8N devem ser utilizados e a lógica de funcionamento do workflow.
