# GUARÁ ↔ ICR | Fronteira pública de integração (sem núcleo)

**Estado:** contrato de arquitetura e checklist para implementação futura. Não declara integração ativa.

## Componentes
- GUARÁ (público): interface do usuário, fluxos institucionais e cenários com dados fictícios.
- Gateway de integração (privado): autenticação, autorização, filtragem de dados, limitação de uso, segregação por organização e logs mínimos.
- ICR Enterprise Runtime (privado): expõe somente operações contratadas e respostas autorizadas.
- ICR Core e Framework operacional (protegidos): **não incluir neste GitHub**, nem em bundles de frontend, commits, images de build, documentação de implementação ou logs.

## Contrato público de capacidades (não é especificação de endpoints reais)
- Verificar status do serviço.
- Abrir ou recuperar uma sessão autorizada.
- Enviar evento/contexto fictício com classificação declarada (fato, hipótese, interpretação ou decisão).
- Recuperar estado e resumo autorizado da continuidade.
- Solicitar relatório/exportação no escopo autorizado.
- Consultar metadados de auditoria disponibilizados segundo política.

**Atenção:** nomes, rotas, schemas e autenticação deverão ser extraídos do contrato real versionado da API, em ambiente restrito. Não presumir que essas operações estão disponíveis na versão atualmente instalada.

## Regras obrigatórias para integração
1. Nenhum segredo, credencial, token, endpoint interno ou chave no cliente web e no GitHub público.
2. Todo acesso via backend/gateway sob HTTPS e autenticação institucional; jamais chamar o Runtime privado diretamente do navegador.
3. Validar tenant, identidade, consentimento, papéis e políticas antes de cada operação.
4. Evitar revelar internals em erros e logs; limitar auditoria a campos autorizados.
5. Não usar dados reais na demonstração pública; não utilizar dados institucionais para treinamento de modelos.
6. Implantação do Runtime em ambiente protegido, com controle de acesso e possibilidade de reversão.
7. Testar isolamento entre organizações, persistência após reinício, autorização, exportação e restauração antes de apresentar como integração concluída.
8. Diferenciar explicitamente na interface três estados: simulado, integrado/testado, indisponível.
9. A autoria e licença do ICR são independentes de contribuições ao GUARÁ; definir isso contratualmente antes de colaboração externa.

## Evidência mínima para ativar a opção 'ICR integrado'
- Identificação e integridade do pacote fechado de implantação validada pelo titular.
- Contrato OpenAPI ou documentação técnica revisada em ambiente privado.
- Gateway com teste de autenticação e de negação de acesso não autorizado.
- Testes de isolamento e consentimento.
- Cenário demonstrável: registrar decisão fictícia, sair, retornar e recuperar corretamente seu contexto.
- Evidência de não exposição do Core em repositórios, artefatos de compilação e respostas HTTP.

## Mensagem pública
O GUARÁ é a aplicação institucional proposta; ICR é sua tecnologia-base de continuidade cognitiva e governança contextual. A demonstração pública atual não executa o ICR Runtime. A integração real será validada somente após acesso controlado ao pacote fechado.
