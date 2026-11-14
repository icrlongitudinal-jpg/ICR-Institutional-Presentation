# GUARÁ + ICR — visão de equivalência funcional com Microsoft 365

## Princípio de apresentação
Objetivo de longo prazo: oferecer capacidades comparáveis ou superiores às de uma plataforma de produtividade institucional, com controle brasileiro de infraestrutura, dados e continuidade contextual.

**Importante:** nenhuma equivalência ou superioridade foi comprovada. A demonstração de sete etapas não é uma substituição funcional do Microsoft 365, não foi homologada pelo governo e não integra o ICR Runtime.

| Área de referência | Capacidade-alvo do GUARÁ | Demonstração atual | Requisito para produto |
| --- | --- | --- | --- |
| Word / Excel / PowerPoint | Editar documentos, planilhas e apresentações | Minuta textual local | Integração com editor compatível; testes de formatos, acessibilidade e colaboração |
| OneDrive | Guardar, versionar e compartilhar arquivos | Referência textual a arquivo | Storage real, cotas, criptografia, versionamento e recuperação |
| SharePoint | Intranet, bibliotecas, fluxos e permissões | Projeto/registro local | Gestão documental, RBAC, workflows e pesquisa |
| Outlook / Exchange | E-mail, contatos, calendário, migração | Mensagens e agenda locais | Servidor e-mail seguro, SMTP/IMAP, antispam, migração, gestão operacional |
| Teams | Chat, canais, áudio/vídeo e reuniões | Mensagens locais | Serviço de chat/vídeo real, gravação controlada, moderação e escalabilidade |
| Entra ID | Identidade, SSO, MFA e diretórios | Ausente | IAM federado, auditoria, MFA, provisionamento e segregação |
| Power Automate | Fluxos e automação | Ausente | Motor de processos com aprovação e política |
| Copilot | Assistência contextual sob autorização | Ausente | Modelos autorizados, governança de IA, avaliações e controles |
| Microsoft Purview / conformidade | Classificação, retenção, eDiscovery e trilhas | Classificação conceitual de registros | Controles formais de retenção, LGPD, auditoria resistente a adulteração |

## Como o ICR se diferencia
- A proposta do ICR é registrar contexto e percurso das decisões humanas, com distinção entre fato, hipótese, interpretação e decisão.
- O GUARÁ é a camada de trabalho institucional que **poderá** utilizar serviços interoperáveis; o Runtime ICR só deve ser apresentado como integrado após teste em ambiente autorizado.
- Interfaces e terminologia próprias: inspiração em requisitos de mercado, **não copiar código, identidade visual, marca nem elementos protegidos da Microsoft**.

## Arquitetura pretendida (não implementada)
Portal GUARÁ → API de serviços / conectores → IAM e colaboração → ICR Runtime privado por interface autorizada → bancos, arquivos, backup e operação sob governança brasileira.

## Etapas de engenharia e validação
1. Contrato de integração ICR e prova de preservação do contexto com dados fictícios.
2. Autenticação institucional, autorização, isolamento de organizações e log verificável.
3. Integração testada de documentos/arquivos, migração, importação/exportação e política de retenção.
4. Correio, agendas e reuniões reais, com métricas de disponibilidade.
5. Testes de segurança, acessibilidade, LGPD, recuperação, desempenho e custos totais.
6. Piloto autorizado com indicadores e relatório de limitações.

## Como avaliar depois de sete etapas
A demonstração permite observar clareza da navegação e representação do fluxo de decisões, não comprova segurança, soberania ou equivalência. Solicitar à avaliadora notas de 1 a 5 para clareza, utilidade, continuidade, confiança e desejo de testar um piloto real; registrar dúvidas e sugestões.

Todos os exemplos precisam ser fictícios. Nenhuma informação da ENAP deve entrar no repositório público.
