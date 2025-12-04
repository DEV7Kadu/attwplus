📱 Whaticket Plus
================

Sistema completo de atendimento e automação para WhatsApp

Version: 28.0.1
API: v7.0.0-rc.9
License: Proprietary
Ubuntu: 22.04

Recursos • Instalação • Changelog • Suporte

---

📋 Índice
-------

- Recursos Principais
- Versões Recentes
- Changelog Completo
- Instalação
- Tecnologias
- Suporte

✨ Recursos Principais
--------------------

🤖 Automação Inteligente:
- Saudação automática em tickets
- Transferência inteligente entre filas
- Sistema de alerta de atendimento
- Notificações automáticas

🔌 Integrações:
- Google Gemini (IA)
- OpenAI GPT (v4.28.0)
- MercadoPago
- Gerencianet

💬 Comunicação Avançada:
- Busca em histórico de mensagens
- Encaminhamento de mensagens
- Reações a mensagens
- Respostas rápidas

👥 Gestão de Grupos:
- Estabilidade aprimorada
- Cache de metadados
- Correção "Invalid public key"
- Decodificação inteligente

🚀 Versões Recentes
------------------

Versão 28.0.1 - 22/11/2025:
API Atualizada: v7.0.0-rc.9

Destaques:
- Atualização crítica da API
- Melhorias de performance
- Correções de bugs menores

Versão 28.0.0 - 15/11/2025:
API Atualizada: v7.0.0-rc.6

Melhorias de Compatibilidade:
- Compatibilidade com Ubuntu 22.04
- Atualização OpenAI API: v3.3.0 → v4.28.0

📚 Changelog Completo
---------------------

Versão 27.0.0 - 13/11/2025:

🔌 Integrações e APIs:
- Integração nativa com Google Gemini
- Novos gateways de pagamento: MercadoPago, Gerencianet
- Configuração via painel administrativo
- API atualizada para v7.0.0-rc.6

🤖 Automação e Atendimento:
- Saudação Automática: Envio ao aceitar tickets
- Notificação de Transferência: Entre filas/agentes
- Alerta de Visualização: Ticket sendo atendido

💬 Mensagens e Comunicação:
+ Busca no histórico de mensagens dentro dos tickets
+ Correção no encaminhamento de mensagens de localização
+ Correção no encaminhamento de arquivos/documentos

🔧 Correção e Normalização de Sessões (JID/LID):

Arquitetura de Identificação:
LID Local ID → Mapeia → JID Phone Number → Garante Compatibilidade
LID Local ID → Elimina → Duplicações
LID Local ID → Preserva → Histórico

Melhorias implementadas:
- Normalização consistente entre envio e recebimento
- Mapeamento automático de LID para JID
- Compatibilidade retroativa garantida
- Tratamento aprimorado de contatos duplicados
- Cache otimizado para melhor desempenho

👥 Decodificação e Confiabilidade em Grupos:

Problema resolvido: Falhas "Invalid public key" em grupos

Soluções implementadas:
1. Patch inteligente para interceptar objetos inválidos
2. Conversão automática de Object() para Buffer
3. Correção de falhas de criptografia
4. Melhoria geral na estabilidade

Resultado: +95% de estabilidade em grupos

⚡ Otimização e Performance:

Melhorias de Performance:
Requisições de Grupo: Alta → Baixa (redução 60%)
Tempo de Carregamento: Lento → Rápido (melhoria 45%)
Uso de Memória: Alto → Otimizado (redução 30%)

Implementações:
- Cache dedicado para metadados de grupos (cachedGroupMetadata)
- Logs de depuração otimizados
- Tratamento de erros aprimorado
- Código refatorado para maior eficiência

🆔 Identificação e Contatos:

Sistema LID (Local ID):
LID: Identificador único e permanente para contatos

Benefícios:
- Independente do número de telefone
- Previne duplicações
- Garante integridade do histórico
- Funciona mesmo após troca de número

🎨 Interface e Experiência do Usuário:

Melhorias visuais:
- Ajuste no menu de anexos (modo escuro)
- Revisão e padronização de nomenclaturas
- Novo design para área de upload
- Botão "Rolar para Baixo" em conversas longas
- Busca avançada em mensagens

Correções:
- Erro "reading includes of null"
- Falhas de renderização na lista de tickets
- Fluidez geral da interface

---

Versão 24.0.0 - 18/07/2025:

🎨 Interface e Temas:
- Modo Escuro: Correções em mensagens
- Botão Light/Dark: Movido para o perfil
- Dashboard: Estilos alterados, botão impressão removido
- Tickets: Estilo ajustado
- Login/Signup: Novo layout

🚀 Funcionalidades:
- Respostas rápidas reformuladas (novo layout)
- Botão de tradução adicionado
- Aviso de contato quando ticket está aberto
- Opção de SuperAdmin no popup de usuário
- Agendamento reformulado com suporte para ciclos
- Correção: permite enviar imagem com texto no agendamento

🔧 Correções Técnicas:
- Correção no envio de menu (filas) - Na terceira tentativa, mensagem enviada automaticamente para primeira fila
- Correção de vazamento no WebSocket
- Correção nos horários de atendimento

---

Versão 23.0.0 - 12/02/2024:

ATENÇÃO: Drive contém plusvipclub.zip com novas correções

📦 Arquivos Corrigidos:
- queues.ts: Envio de texto + imagem nas campanhas
- SendWhatsAppMedia.ts: Envio de áudio em respostas rápidas
- wbotMessageListener.ts: Correção de MENU duplicado

🔧 Correções Implementadas:
- Envio de mídia na fila: QueueOptionController.ts, QueueController.ts, wbotMessageListener.ts
- Erro de digitação no Contact (Linha 2108)
- Remoção da verificação baseada em regex
- Qualquer entrada numérica válida agora é aceita

---

Versão 22.0.0 - 13/11/2024:

🔧 Correções e Melhorias:

Correções Principais:
- Redimensionamento da área de ticket
- toastError.js corrigido
- Validação do número no ContactModal
- OpenAI atualizado para v3.3.0
- Avaliações de 1 a 5 estrelas
- Mensagem de avaliação (apenas em atendimento)

Implementações:
- Horários intercalados
- Logo alternativo (Light/Dark)
- Kanban inserido e reformulado
- Fix áudio no iPhone
- Chat no modo Dark corrigido
- Pastas por empresas na "public"

---

Versão 21.0.0 - 07/11/2024:

🔧 Correções:
- Data de vencimento no topo permanece fixa
- Automação não envia para grupos
- Botão disableBot para desabilitar bots/automações
- Correção de mensagem citada
- Permissão para conexões com mesmo nome
- Correção no envio de áudio OGG

🚀 Funcionalidades:

Gestão de Empresas:
- Expiração de conexões após vencimento
- Atualização financeira automática após alteração de plano

Gestão de Contatos:
- Seleção para deletar contatos em massa
- Remoção de abas desnecessárias no painel de usuários

---

Versão 20.0.0 - 31/08/2024:

🆕 Novidades:

Recursos de Mensagens:
- Fechar todos os tickets (abertos ou em espera)
- Reagir a mensagens
- Encaminhar mensagens para outro ticket
- Notificação de mensagem apagada

Interface:
- Menu aprimorado
- Botão "Sair" no menu
- Novo layout de login
- Indicação "Digitando" ou "Gravando" no ticket

---

Versão 19.0.0 - 24/07/2024:

🔧 Correções e Melhorias:

Funcionalidades de Usuário:
- Correção no Vcard
- Habilitar/desabilitar novos registros
- Tempo de Trial no painel
- Respostas rápidas para todos os usuários
- Status do número e última interação
- Visualização do número conectado
- Botão para reiniciar conexões
- Alterar logo pelo painel

Administração:
- Nova aba: Cadastrar Empresa
- Opção de Plano Interno

---

🛠️ Instalação
------------

Pré-requisitos:
- Ubuntu 22.04 LTS
- Node.js 18+
- PostgreSQL 14+
- Redis 6+

Instalação Rápida:
# Clone o repositório
git clone https://github.com/seu-usuario/whaticket-plus.git

# Entre no diretório
cd whaticket-plus

# Execute o script de instalação
./install.sh

Atualização:
# Execute o script de atualização
./wplusatualizar.sh

Importante: Sempre faça backup antes de atualizar!

🔧 Tecnologias
-------------

Node.js • React • TypeScript • PostgreSQL • Redis

Stack Completo:
- Backend: Node.js + TypeScript + Express
- Frontend: React + Material-UI
- Banco de Dados: PostgreSQL + Sequelize ORM
- Cache: Redis
- WebSocket: Socket.io
- IA: OpenAI GPT-4 + Google Gemini

📞 Suporte
---------

Precisa de ajuda?
Discord: https://discord.gg/seu-servidor
Telegram: https://t.me/seu-grupo
Email: suporte@whaticketplus.com

📖 Documentação:
- Wiki Completa: https://github.com/seu-usuario/whaticket-plus/wiki
- Tutoriais: https://github.com/seu-usuario/whaticket-plus/wiki/tutorials
- FAQ: https://github.com/seu-usuario/whaticket-plus/wiki/faq

📊 Estatísticas:
GitHub stars • GitHub forks • GitHub watchers

📄 Licença
---------

Copyright © 2024 Whaticket Plus. Todos os direitos reservados.

Este é um software proprietário. O uso, cópia, modificação e/ou distribuição não autorizada é estritamente proibida.

---

Feito com ❤️ para otimizar seu atendimento no WhatsApp

⬆ Voltar ao topo
