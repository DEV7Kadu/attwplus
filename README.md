# 📝 Log de Versões - Whaticket Plus

## 🚀 Versão 24.0.0 - 16/04/2025

✅ Correções no Darkmode (em mensagens)
✅ Botão Light/Dark movido (agora localizado no perfil)
✅ Estilos dos cards da Dashboard alterados (botão de impressão removido)
✅ Estilo de tickets ajustado
✅ Respostas rápidas reformuladas (novo layout)
✅ Correção no envio de menu (filas) – na terceira tentativa, a mensagem é enviada automaticamente para a primeira fila.
✅ Botão de tradução adicionado
✅ Aviso de contato (quando o ticket está aberto, um aviso é emitido)
✅ Página de conexão redesenhada
✅ Inclusão da opção de SuperAdmin (no popup de usuário)
✅ Correção de agendamento (agora permite enviar imagem junto ao texto)
✅ Agendamento reformulado (suporte para ciclos adicionado)
✅ Novo layout das telas de login e signup
✅ Correção de vazamento no WebSocket
✅ Correção nos Horarios de Atendimento

## 🚀 Versão 23.0.0 - 12/02/2024 (11:38)

ATENÇÃO: Drive contem plusvipclub.zip com novas correções e github também:
Arquivos corrigidos: queues.ts (Envio de texto + img nas campanhas); SendWhatsAppMedia.ts (Envio de Audio em respota rapidas); wbotMessageListener.ts (Correção MENU duplicado).

*Faça a atualização seguindo passo a passo do wplusatualizar.sh

FIX: Envio de midia na fila (QueueOptionController.ts, QueueController.ts, wbotMessageListener.ts)
FIX: ,Contact (Erro de digitação) "Linha 2108: const body = `\u200e ${whatsapp.outOfHoursMessage}`;" (wbotMessageListener.ts)

Correção do envio de fila WHATICKET:

Removemos a verificação baseada em regex que impedia a seleção de filas após uma mensagem inválida. Agora, qualquer entrada numérica válida é aceita, independente da última mensagem enviada pelo bot.


## 🚀 Versão 22.0.0 - 13/11/2024 (13:17)

✅ Correção ao Redimensionar Área de Ticket: Erro corrigido ao redimensionar.  
✅ Correção de toastError.js: Problema resolvido no `toastError.js`.  
✅ Validação do Número no ContactModal: Validação aprimorada.  
✅ Atualização OpenAI: Atualização para versão "openai": "3.3.0" e wbotMessageListener.ts.  
✅ Correção nas Avaliações de 1 para 5: Ajuste nas avaliações de 1 a 5 estrelas.  
✅ Mensagem de Avaliação Somente Quando o Ticket Estiver em Atendimento: Avaliações só aparecem quando o ticket está ativo.  
✅ Horários Intercalados: Implementação de horários intercalados.  
✅ Alteração de LOGO de Acordo com LIGHT e DARK: Logo ajustado conforme o tema.  
✅ Inserido no Kanban e Reformulado
✅ Fix Audio no iPhone (Não estava reproduzindo)
✅ Correção Chat no modo Dark
✅ Inserido pastas por empresas na "public"

## 🚀 Versão 21.0.0 - 07/11/2024

✅ Correção da Data de Vencimento no Topo: A data agora permanece fixa.  
✅ Automação em Grupos: Não envia automações para grupos.  
✅ Botão `disableBot`: Desabilita bots ou automações.  
✅ Correção de Mensagem Citada: Erro corrigido nas mensagens citadas.  
✅ Permissão para Conexões com Mesmo Nome: Permite conexões com o mesmo nome.  
✅ Expiração de Conexões: Desconexão automática após vencimento da empresa.  
✅ Seleção para Deletar Contatos: Opção de seleção para exclusão na página "Contatos".  
✅ Correção no Envio de Áudio OGG em Respostas Rápidas: Envio de áudios corrigido.  
✅ Visualização de Tickets Fechados por Operador: Aba removida do painel de usuários.  
✅ Visualização de Grupos por Operador: Aba removida do painel de usuários.  
✅ Atualização Financeira após Alteração de Plano: Valor ajustado automaticamente na lista do Financeiro.

## 🚀 Versão 20.0.0 - 31/08/2024

✅ Fechar todos os tickets abertos ou em espera.
✅ Reagir a uma mensagem.
✅ Encaminhar mensagens para outro ticket.
✅ Aparência do menu aprimorada.
✅ Botão “Sair” adicionado ao menu.
✅ Notificação quando uma mensagem é apagada no WhatsApp, informando no chat.
✅ API atualizada.
✅ Novo layout da página de login.
✅ Indicação “Digitando” ou “Gravando” aparece no ticket, no canto inferior direito, ao lado do nome.

## 🚀 Versão 19.0.0 - 24/07/2024

✅ Fizemos correção no Vcard
✅ Função de habilitar e desabilitar novos registros
✅ Tempo de Trial disponível no Painel
✅Respostas rápidas visualizadas por todos os usuários
✅ Contatos agora aparece se é um número ok e o horário da última interação
✅ Agora é possível ver o número que está conectado no Whaticket
✅ Botão para reiniciar conexões adicionado
✅ Alterar logo pelo Painel
✅ Adicionado nova ABA Cadastrar Empresa
✅ Add Opção Plano Interno
