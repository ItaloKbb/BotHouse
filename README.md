# 🏠 BotHouse - Plataforma Open-Source de Assistência Virtual Inteligente

**Personagens 3D interativos que entendem contexto e reconhecem usuários para oferecer assistência personalizada**

## 🌟 Visão do Projeto
Criar assistentes virtuais que vão além do chat tradicional: personagens 3D animados que entendem contexto, reconhecem usuários individualmente e oferecem interações personalizadas para resolver problemas reais.

## 🚀 Recursos Principais
- **👤 Personagens 3D Inteligentes**: Modelos animados com reações contextuais
- **🔍 Reconhecimento de Usuários**: Diferencia membros da mesma casa (ex: Maria vs João)
- **🎤 Análise de Emoção por Voz**: Detecta sentimentos e adapta respostas
- **🔐 Autenticação Segura**: Sistema JWT com contexto por household
- **📱 PWA Moderno**: Acessível em qualquer dispositivo
- **🧠 Núcleo Conversacional Avançado**: Baseado em Rasa Open Source

## 💡 Casos de Uso
- **Idosos**: Companhia interativa e lembretes de medicamentos
- **Educação**: Tutor virtual para auxílio nos estudos
- **Saúde Mental**: Acompanhamento emocional com respostas empáticas
- **Produtividade**: Assistente pessoal para organização de tarefas

## 🛠 Stack Tecnológica
```mermaid
graph LR
PWA[Frontend PWA] -->|HTTPS| GW[API Gateway]
PWA -->|WebSocket| RASA[Rasa Server]
GW --> AUTH[Auth Service]
GW --> VOICE[Voice Analysis]
GW --> USER[User Service]
RASA --> DB[(PostgreSQL)]
VOICE --> DB
USER --> DB
