Okay, compreendido! Com base nos PDFs ("Declaração de Idoneidade" e "Formulário de Solicitação de Registro") e nas informações detalhadas sobre o processo da CBRR, vamos criar wireframes mais específicos e completos para as telas do sistema web.

Considerando a quantidade de informações no "Formulário de Solicitação de Registro", a abordagem mais adequada será um **formulário multi-etapas** para não sobrecarregar o usuário em uma única tela.

---

## Wireframes Detalhados - Sistema de Registro CBRR

**Observação:** Estes wireframes são de baixa/média fidelidade, focando na estrutura, conteúdo e fluxo, não no design visual final. Elementos como `[ ]` representam checkboxes, `( )` representam radio buttons, e `[ Campo de Texto ]` representa inputs.

---

**Wireframe 1: Tela de Login / Criação de Conta Inicial**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Sistema de Registro Profissional         |
+----------------------------------------------------------+
|                                                          |
|      **Acesso ao Sistema / Criar Conta**                 |
|                                                          |
|      [----- Login -----]    [----- Criar Conta -----]    |
|                                                          |
|      **Criar Conta:**                                    |
|      Email:                                              |
|      [ Campo de Texto: seuemail@exemplo.com________ ]    |
|      Senha:                                              |
|      [ Campo de Senha: ************____________ ]        |
|      Confirmar Senha:                                    |
|      [ Campo de Senha: ************____________ ]        |
|                                                          |
|      [ ] Li e aceito os Termos de Uso preliminares       |
|                                                          |
|                     +-----------------+                  |
|                     |   Criar Conta   |                  |
|                     +-----------------+                  |
|                                                          |
|      *Após criar a conta, você será direcionado para     |
|      o preenchimento do formulário de solicitação.*      |
|                                                          |
+----------------------------------------------------------+
```

---

**Wireframe 2: Dashboard Principal do Usuário (Após Login)**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Sistema de Registro - Olá, [Nome Usuário]|
+----------------------------------------------------------+
| [Dashboard] [Minha Solicitação] [Meus Dados] [Sair]      |
+----------------------------------------------------------+
|                                                          |
|  **Status da sua Solicitação de Registro PQR.CBRR**      |
|                                                          |
|  *Progresso:*                                            |
|  [Formulário] -> [Docs] -> [Pgto] -> [Análise CBRR] -> [Finalizado] |
|  (Barra de progresso visual aqui)                        |
|                                                          |
|  *Status Atual:*                                         |
|  **[ Formulário Incompleto ] ✏️**                       |
|  (Ou: Aguardando Documentos, Aguardando Pagamento,       |
|   Em Análise ⏳, Aprovado ✔️, Reprovado ❌, Pendente Correção ⚠️) |
|                                                          |
|  *Próxima Ação:*                                         |
|  [ Continuar Preenchimento do Formulário ]               |
|  (Ou: Enviar Documentos Pendentes, Enviar Comprovante...) |
|                                                          |
|  *Notificações Recentes:*                                |
|  - DD/MM/AAAA: E-mail de boas-vindas enviado.            |
|  - ...                                                   |
|                                                          |
+----------------------------------------------------------+
```

---

**Wireframe 3: Formulário de Solicitação - Etapa 1: Dados Pessoais e Identificação**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Formulário de Solicitação - Etapa 1/8    |
+----------------------------------------------------------+
| [Anterior] . . . . . . . . . . . . . . . [Próximo >]    |
+----------------------------------------------------------+
|                                                          |
|  **1. Dados Pessoais**                                   |
|  Nome Completo: [ Campo: Nome Conforme ID______________ ] |
|  Endereço: [ Campo: Rua, Nº, Comp______________________ ] |
|  Bairro: [ Campo: Bairro_______________________________ ] |
|  Cidade: [ Campo: Cidade________________ ] UF: [ Sel: UF ]|
|  CEP: [ Campo: XXXXX-XXX____ ] País: [ Campo: Brasil____ ]|
|  Telefone Celular: [ Campo: (XX) XXXXX-XXXX ]            |
|  Telefone Fixo: [ Campo: (XX) XXXX-XXXX__ ]              |
|  Email: [ Campo: email@preenchido.com (somente leitura)] |
|  Data de Nascimento: [ Campo Data: DD/MM/AAAA ]          |
|  Local de Nascimento: [ Campo: Cidade/UF/País__________ ]|
|  Nacionalidade: [ Campo: Brasileira____________________ ]|
|                                                          |
|  **2. Documentos de Identificação**                      |
|  *Documento Principal (RG ou Passaporte p/ Estrangeiros)* |
|  Tipo: [ Sel: RG / Passaporte ]                          |
|  Número: [ Campo: Número ID__________ ]                  |
|  Órgão Emissor/SSP: [ Campo: SSP/UF ou Órgão ]           |
|  Data de Emissão: [ Campo Data: DD/MM/AAAA ]             |
|                                                          |
|  *CPF (Obrigatório para Brasileiros)*                    |
|  Número CPF: [ Campo: XXX.XXX.XXX-XX_________ ]          |
|                                                          |
|  *Registro Profissional (CREA, etc.)*                    |
|  Conselho: [ Campo: CREA/Outro_________ ] Nº: [ Campo Nº ]|
|  Data de Emissão: [ Campo Data: DD/MM/AAAA ]             |
|  UF Registro: [ Sel: UF ]                                |
|                                                          |
|                      +---------------+                   |
|                      |   Próximo >   |                   |
|                      +---------------+                   |
+----------------------------------------------------------+
```

---

**Wireframe 4: Formulário de Solicitação - Etapa 2: Formação Acadêmica e Associações**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Formulário de Solicitação - Etapa 2/8    |
+----------------------------------------------------------+
| [< Anterior] . . . . . . . . . . . . . . [Próximo >]    |
+----------------------------------------------------------+
|                                                          |
|  **3. Formação Acadêmica**                               |
|  *Adicione suas formações (Graduação e Pós-Graduação)*   |
|  +---------------------------------------------------+   |
|  | Título: [ Campo: Engenharia de Minas____________ ] |   |
|  | Instituição: [ Campo: Universidade Exemplo______ ] |   |
|  | Ano de Conclusão: [ Campo Ano: AAAA ] [Excluir -] |   |
|  +---------------------------------------------------+   |
|  +---------------------------------------------------+   |
|  | Título: [ Campo: Mestrado em Geologia__________ ] |   |
|  | Instituição: [ Campo: Instituto XYZ_____________ ] |   |
|  | Ano de Conclusão: [ Campo Ano: AAAA ] [Excluir -] |   |
|  +---------------------------------------------------+   |
|                    [ + Adicionar Formação ]              |
|                                                          |
|  **4. Outras Associações Profissionais**                 |
|  *Liste outras associações relevantes (opcional)*        |
|  +---------------------------------------------------+   |
|  | Associação: [ Campo: Nome Associação___________ ] |   |
|  | Número: [ Campo: Nº Assoc_______ ]                |   |
|  | Data Filiação: [ Campo Data: DD/MM/AAAA ]         |   |
|  | Categoria: [ Campo: Tipo Membro_____ ] [Excluir -]|   |
|  +---------------------------------------------------+   |
|                 [ + Adicionar Associação ]               |
|                                                          |
|                      +---------------+                   |
|                      |   Próximo >   |                   |
|                      +---------------+                   |
+----------------------------------------------------------+
```

---

**Wireframe 5: Formulário de Solicitação - Etapa 3: Áreas de Competência e Checklist**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Formulário de Solicitação - Etapa 3/8    |
+----------------------------------------------------------+
| [< Anterior] . . . . . . . . . . . . . . [Próximo >]    |
+----------------------------------------------------------+
|                                                          |
|  **5. Áreas de Competência do Registro**                 |
|  *Assinale as áreas para as quais solicita registro:*    |
|  [ ] 1. Exploração Mineral                              |
|  [ ] 2. Estimativa de Recursos Minerais                 |
|  [ ] 3. Estimativa de Reservas Minerais                 |
|  [ ] 4. Operações de Mineração                          |
|  [ ] 5. Processamento Mineral                           |
|  [ ] 6. Meio Ambiente e Sustentabilidade                |
|  [ ] 7. Avaliação Econômico-Financeira de Ativos Min.   |
|  [ ] 8. Regulação Minerária do Brasil                   |
|  [ ] 9. Geotecnia                                       |
|      *Se Geotecnia, especifique a(s) área(s) de atuação:*|
|      [ ] Barragens [ ] Pilhas [ ] Mina Céu Aberto [ ] Mina Subt.|
|                                                          |
|  *Bens minerais relacionados às áreas de competência:*   |
|  [ Área de Texto: Liste os bens minerais (Ouro, Ferro...)] |
|                                                          |
|  **6. Lista de Verificação (Requisitos Essenciais)**      |
|  *Confirme que você atende aos seguintes requisitos:*    |
|  [ ] Possuo curso universitário concluído (Brasil/Exterior Rec.) |
|  [ ] Possuo pelo menos 10 anos de experiência no setor mineral |
|  [ ] Possuo pelo menos 5 anos de experiência relevante no(s) tipo(s) de depósito/operação e área(s) de competência selecionada(s) |
|  [ ] Ocupei Posição de Responsabilidade (participação essencial em decisões) por pelo menos 3 anos em cada competência requerida |
|  [ ] Possuo registro profissional válido e quite no Brasil |
|  [ ] Li e compreendi o Regulamento do Comitê [Link]     |
|  [ ] Li e compreendi o Código de Ética CBRR [Link]        |
|  [ ] Li e compreendi o Guia CBRR [Link]                   |
|                                                          |
|                      +---------------+                   |
|                      |   Próximo >   |                   |
|                      +---------------+                   |
+----------------------------------------------------------+
```

---

**Wireframe 6: Formulário de Solicitação - Etapa 4: Experiência Profissional**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Formulário de Solicitação - Etapa 4/8    |
+----------------------------------------------------------+
| [< Anterior] . . . . . . . . . . . . . . [Próximo >]    |
+----------------------------------------------------------+
|                                                          |
|  **7. Experiência Profissional**                         |
|  *Detalhe suas experiências relevantes (mínimo 10 anos)* |
|  +---------------------------------------------------+   |
|  | Nome da Empresa/Instituição: [ Campo __________ ] |   |
|  | Endereço: [ Campo _____________________________ ] |   |
|  | Período: [ Data Início ] a [ Data Fim ou Atual ]  |   |
|  | Cargos Ocupados: [ Campo _______________________ ] |   |
|  | Descrição Atividades (Responsabilidades, equipe,   |   |
|  | orçamento, Posição de Responsabilidade):          |   |
|  | [ Área de Texto Detalhada _____________________ ] |   |
|  | Contato para Comprovação (Nome/Email/Telefone):   |   |
|  | [ Campo _______________________________________ ] |   |
|  |                                     [Excluir -] |   |
|  +---------------------------------------------------+   |
|               [ + Adicionar Experiência Profissional ]   |
|                                                          |
|                      +---------------+                   |
|                      |   Próximo >   |                   |
|                      +---------------+                   |
+----------------------------------------------------------+
```

---

**Wireframe 7: Formulário de Solicitação - Etapa 5: Exp. Acadêmica, Publicações, Relatórios**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Formulário de Solicitação - Etapa 5/8    |
+----------------------------------------------------------+
| [< Anterior] . . . . . . . . . . . . . . [Próximo >]    |
+----------------------------------------------------------+
|                                                          |
|  **8. Experiência Acadêmica (Pesquisa/Ensino)**          |
|  +---------------------------------------------------+   |
|  | Curso Ministrado/Título Pesquisa: [ Campo ______ ] |   |
|  | Instituição: [ Campo ___________________________ ] |   |
|  | Período: [ Data Início ] a [ Data Fim ou Atual ]  |   |
|  |                                     [Excluir -] |   |
|  +---------------------------------------------------+   |
|              [ + Adicionar Experiência Acadêmica ]       |
|                                                          |
|  **9. Publicações**                                      |
|  +---------------------------------------------------+   |
|  | Título Artigo/Livro: [ Campo ___________________ ] |   |
|  | Nome da Publicação/Editora: [ Campo ____________ ] |   |
|  | Data Publicação: [ Campo Data: MM/AAAA ]          |   |
|  |                                     [Excluir -] |   |
|  +---------------------------------------------------+   |
|                      [ + Adicionar Publicação ]          |
|                                                          |
|  **10. Relatórios Técnicos Relevantes**                  |
|  +---------------------------------------------------+   |
|  | Tipo (Público, Interno, etc.): [ Campo __________ ] |   |
|  | Data Publicação: [ Campo Data: MM/AAAA ]          |   |
|  | Área de Responsabilidade: [ Campo ______________ ] |   |
|  | Descrição Sucinta (Resp. Principal/Parcial):      |   |
|  | [ Área de Texto Curta _________________________ ] |   |
|  |                                     [Excluir -] |   |
|  +---------------------------------------------------+   |
|                   [ + Adicionar Relatório Técnico ]      |
|                                                          |
|                      +---------------+                   |
|                      |   Próximo >   |                   |
|                      +---------------+                   |
+----------------------------------------------------------+
```

---

**Wireframe 8: Formulário de Solicitação - Etapa 6: Outras Experiências e Referências**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Formulário de Solicitação - Etapa 6/8    |
+----------------------------------------------------------+
| [< Anterior] . . . . . . . . . . . . . . [Próximo >]    |
+----------------------------------------------------------+
|                                                          |
|  **11. Outras Experiências e Atividades Relevantes**     |
|  *Descreva outras informações pertinentes à sua qualificação*|
|  [ Área de Texto Ampla _______________________________ ] |
|  [ ___________________________________________________ ] |
|                                                          |
|  **12. Referências Profissionais (*Mínimo 3*)**          |
|  +---------------------------------------------------+   |
|  | Nome: [ Campo Completo__________________________ ] |   |
|  | Ocupação/Cargo: [ Campo ________________________ ] |   |
|  | Email: [ Campo Email____________________________ ] |   |
|  | Telefone (Celular e/ou Fixo): [ Campo __________ ] |   |
|  |                                     [Excluir -] |   |
|  +---------------------------------------------------+   |
|  +---------------------------------------------------+   |
|  | Nome: [ Campo Completo__________________________ ] |   |
|  | ... (repetir campos) ...                        |   |
|  |                                     [Excluir -] |   |
|  +---------------------------------------------------+   |
|  +---------------------------------------------------+   |
|  | Nome: [ Campo Completo__________________________ ] |   |
|  | ... (repetir campos) ...                        |   |
|  |                                     [Excluir -] |   |
|  +---------------------------------------------------+   |
|                      [ + Adicionar Referência ]          |
|                                                          |
|                      +---------------+                   |
|                      |   Próximo >   |                   |
|                      +---------------+                   |
+----------------------------------------------------------+
```

---

**Wireframe 9: Formulário de Solicitação - Etapa 7: Declaração de Idoneidade**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Formulário de Solicitação - Etapa 7/8    |
+----------------------------------------------------------+
| [< Anterior] . . . . . . . . . . . . . . [Próximo >]    |
+----------------------------------------------------------+
|                                                          |
|  **13. Declaração de Idoneidade**                        |
|  *Revise e confirme as informações abaixo:*              |
|                                                          |
|  Eu, **[Nome Completo - Preenchido Automático]**,        |
|  brasileiro(a), estado civil [ Campo: Estado Civil ],    |
|  nascido(a) em [ Data Nasc - Automático ] / [ Local Nasc - Automático ], |
|  na cidade de [ Cidade Nasc - Automático ], UF [ UF Nasc - Automático ], |
|  documento de identidade tipo [ Tipo ID - Automático ]   |
|  nº [ Nº ID - Automático ], SSP/ [ Órgão Emissor - Automático ], |
|  emitido em [ Data Emissão ID - Automático ], residente à |
|  Rua/Av. [ Endereço - Automático ], Nº [ Número End - Automático ], |
|  Bairro [ Bairro - Automático ], na cidade de            |
|  [ Cidade End - Automático ], UF [ UF End - Automático ], |
|  CPF nº [ CPF - Automático ], DECLARO, sob as penas da   |
|  Lei... (continuar texto completo da declaração aqui)    |
|  ...ficarei sujeito (a) à exclusão... aplicáveis.        |
|                                                          |
|  Desde já, autorizo a CBRR a buscar informações          |
|  complementares sobre minha pessoa.                      |
|                                                          |
|  A presente declaração é feita, sob as penas da lei, como|
|  verdadeira.                                             |
|                                                          |
|  [ ] **Confirmo que li, compreendi e concordo com os**   |
|      **termos desta Declaração de Idoneidade, e que as** |
|      **informações apresentadas são verdadeiras.**       |
|      **(Esta marcação equivale à sua assinatura digital)**|
|                                                          |
|                      +---------------+                   |
|                      |   Próximo >   |                   |
|                      +---------------+                   |
+----------------------------------------------------------+
```

---

**Wireframe 10: Formulário de Solicitação - Etapa 8: Upload de Documentos**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Formulário de Solicitação - Etapa 8/8    |
+----------------------------------------------------------+
| [< Anterior] . . . . . . . . . . . . . . [Finalizar e Enviar] |
+----------------------------------------------------------+
|                                                          |
|  **14. Anexar Documentos Obrigatórios**                  |
|  *Formatos aceitos: PDF, JPG, PNG. Tamanho máx: 5MB/arq* |
|                                                          |
|  - Cópia do Documento Válido (ID ou Passaporte):         |
|    [ Botão Upload Doc ID ] [ status: Nenhum arquivo ]    |
|  - Cópia Carteira Registro Profissional:                 |
|    [ Botão Upload Reg Prof ] [ status: Enviado: nome.pdf X ]|
|  - Comprovante Quitação Anuidade Registro Profissional:  |
|    [ Botão Upload Anuidade ] [ status: Nenhum arquivo ]  |
|  - Certificado(s) Graduação Universitária:               |
|    [ Botão Upload Graduação ] [ status: Nenhum arquivo ] |
|    (Permitir múltiplos uploads para este item)           |
|  - Certificado(s) Pós-Graduação (se aplicável):          |
|    [ Botão Upload Pos Grad ] [ status: Nenhum arquivo ]  |
|    (Permitir múltiplos uploads)                          |
|  - Currículo Profissional (Histórico Profissional):      |
|    [ Botão Upload CV ] [ status: Nenhum arquivo ]        |
|  - Declaração de Idoneidade (Você confirmou na etapa anterior)|
|    *(Não requer upload, apenas confirmação)*             |
|                                                          |
|  **15. Pagamento da Taxa de Submissão (R$ 50,00)**       |
|  *Realize o pagamento e anexe o comprovante.*            |
|  Dados para Transferência/Depósito:                      |
|  Banco do Brasil (001) / Ag: 1607-1 / CC: 405131-9       |
|  CNPJ: 25.277.283/0001-44 / CBRR                         |
|  *Ou solicite Boleto: registro@cbrr.org.br (anexar aqui)*|
|                                                          |
|  - Comprovante de Pagamento Taxa CBRR:                   |
|    [ Botão Upload Compr Pgto ] [ status: Nenhum arquivo ]|
|                                                          |
|  **16. Declarações Finais**                              |
|  [ ] Declaro ter lido e compreendido o ESTATUTO CBRR [Link]|
|  [ ] Declaro ter lido e compreendido o CÓDIGO DE ÉTICA CBRR [Link]|
|  [ ] Declaro ter lido e compreendido o GUIA CBRR [Link]   |
|  [ ] Assumo a responsabilidade pelo conteúdo de Relatórios|
|      Técnicos assinados por mim.                         |
|                                                          |
|                 +-------------------------+              |
|                 | Finalizar e Enviar Tudo |              |
|                 +-------------------------+              |
+----------------------------------------------------------+
```

---

**Wireframe 11: Tela de Status do Processo (Usuário - Detalhada)**

*Similar ao Wireframe 2 (Dashboard), mas focado apenas no processo após envio.*

```
+----------------------------------------------------------+
| [Logotipo CBRR] Sistema de Registro - Olá, [Nome Usuário]|
+----------------------------------------------------------+
| [Dashboard] [Minha Solicitação] [Meus Dados] [Sair]      |
+----------------------------------------------------------+
|                                                          |
|  **Acompanhamento - Solicitação PQR.CBRR**               |
|                                                          |
|  *Progresso:*                                            |
|  [Formulário ✔] -> [Docs ✔] -> [Pgto ✔] -> [Análise CBRR ⏳] -> [Finalizado] |
|  (Barra de progresso visual aqui)                        |
|                                                          |
|  *Status Atual:*                                         |
|  **[ Em Análise pelo Comitê de Registro ] ⏳**           |
|  *(Previsão de resposta em até 60 dias)*                 |
|  (Ou: Aprovado ✔️, Reprovado ❌, Correção Necessária ⚠️)  |
|                                                          |
|  *Detalhes da Submissão:*                                |
|  - Data de Envio Completo: DD/MM/AAAA HH:MM              |
|  - [ Link: Visualizar Formulário Enviado ]               |
|  - [ Link: Ver Documentos Enviados ]                     |
|                                                          |
|  *Histórico e Comunicações:*                             |
|  - DD/MM/AAAA: Solicitação e documentos recebidos.       |
|  - DD/MM/AAAA: Confirmação de recebimento enviada p/ email.|
|  - [Se houver Correção]:                                 |
|    *Comunicação do Comitê (DD/MM/AAAA):*                 |
|    "Prezado(a) [Nome], favor reenviar o comprovante de   |
|     quitação da anuidade profissional (arquivo ilegível)."|
|    [ Botão: Enviar Documento Corrigido ]                 |
|  - [Se Aprovado/Reprovado]:                              |
|    *Decisão do Comitê (DD/MM/AAAA):*                     |
|    "Sua solicitação foi Aprovada." (ou Reprovada/Motivo) |
|                                                          |
+----------------------------------------------------------+
```

---

**Wireframe 12: Painel de Avaliação do Comitê (Adaptado)**

```
+----------------------------------------------------------+
| [Logotipo CBRR] Painel do Comitê de Registro             |
+----------------------------------------------------------+
| [Pendências] [Em Análise] [Histórico] [Config.] [Sair]   |
+----------------------------------------------------------+
|                                                          |
|  **Avaliação de Solicitação de Registro PQR.CBRR**       |
|  Solicitante: [Nome Completo Usuário] | ID Solic: [XXXXX]|
|  Data Submissão: [DD/MM/AAAA] | Status: [ Em Análise ]   |
|                                                          |
|  **Verificar Informações e Documentos:**                 |
|  [ Seção: Dados Pessoais e Identificação ] [+] Expandir  |
|  [ Seção: Formação Acadêmica e Associações ] [+] Expandir|
|  [ Seção: Áreas Competência e Checklist ] [+] Expandir   |
|      - Áreas Solicitadas: [Lista das áreas marcadas]     |
|      - Checklist Requisitos: [Verificar marcações do user]|
|  [ Seção: Experiência Profissional ] [+] Expandir        |
|      - Anos Totais Calculados: [Sistema calcula/exibe]   |
|      - Anos Posição Responsabilidade: [Sistema calcula]  |
|  [ Seção: Exp. Acadêmica, Publicações, Relatórios ] [+] Expandir |
|  [ Seção: Outras Experiências e Referências ] [+] Expandir|
|  [ Seção: Declaração de Idoneidade ] [ Ver Confirmação ] |
|  [ Seção: Documentos Anexados ]                          |
|      - Doc ID: [Link Ver/Baixar] [ Status Validação? OK/!] |
|      - Reg. Profissional: [Link Ver/Baixar] [ Status? OK/!] |
|      - Anuidade: [Link Ver/Baixar] [ Status? OK/!]       |
|      - Graduação: [Link Ver/Baixar] [ Status? OK/!]      |
|      - Pós (se houver): [Link Ver/Baixar] [ Status? OK/!] |
|      - CV: [Link Ver/Baixar] [ Status? OK/!]             |
|      - Compr. Pagamento: [Link Ver/Baixar] [ Status? OK/!] |
|  [ Seção: Declarações Finais ] [ Ver Confirmações ]      |
|                                                          |
|  **Ação do Comitê:**                                     |
|  ( ) Aprovar Registro PQR.CBRR nas áreas: [Selecionar áreas]|
|  ( ) Reprovar Solicitação                                |
|  ( ) Solicitar Correção / Informação Adicional           |
|                                                          |
|  *Justificativa / Feedback (Interno e/ou para Solicitante):*|
|  [ Área de Texto para Comentários da Comissão _________ ] |
|  [ ] Enviar este comentário ao solicitante por e-mail    |
|                                                          |
|           +----------------------+                       |
|           | Registrar Decisão    |                       |
|           +----------------------+                       |
|           [ Salvar Rascunho ] [ Voltar para Lista ]      |
+----------------------------------------------------------+
```

---

Esses wireframes detalhados refletem as informações específicas do processo CBRR e a estrutura necessária para coletar todos os dados e documentos de forma organizada através do sistema web.
