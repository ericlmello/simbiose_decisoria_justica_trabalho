Desenho Atento

Pontos de verificação na interface para supervisão humana real sobre sistemas preditivos judiciais

Proposta institucional submetida ao programa Artesãos da Inovação do TRT-2 (Tribunal Regional do Trabalho da 2ª Região), com a camada técnica de rastreamento e avaliação de metas que sustenta a esteira de dados por trás dos painéis preditivos (PAI, módulos do e-Gestão).

O problema

O TRT-2 apoia-se cada vez mais em painéis de avaliação e previsão de produção. Isso expõe uma dupla vulnerabilidade institucional:

Viés de automação. Sob alta pressão, gestores e magistrados tendem a aceitar alertas e previsões sistêmicas de forma acrítica, perdendo a capacidade de identificar erros silenciosos na predição.
Shadow AI. Sem ferramenta corporativa própria de IA generativa, o art. 19 da Resolução CNJ nº 615/2025 faculta o uso de soluções externas sob condições (anonimização, dever de informar o Tribunal). A única via de captura desse uso hoje é a autodeclaração, sem verificação independente.
A solução

A proposta separa a interação em duas camadas, cada uma tratada por uma técnica oposta:

Camada de acesso: sem fricção. O canal oficial precisa ser rápido o bastante para competir com ferramentas externas.
Camada de decisão: fricção deliberada. Só nas tarefas de alto risco (AR1 a AR5 da Resolução 615), a recomendação exige um ato deliberado para ser exibida, com a origem do material sempre visível ("De onde veio isto").

Essa camada de decisão é alimentada por rastreamento técnico automático da esteira de dados (jobs sequenciais de Staging e Remessa Diária): cada execução recebe um identificador único, cada etapa registra sua origem e um resumo criptográfico do dado processado, e a volumetria captada alimenta uma avaliação automatizada de aderência a metas de produção, sem coleta manual.

Neste repositório
Arquivo	Descrição
proposta_desenho_atento.docx	Texto completo da proposta institucional
pentaho_pipeline_retry.py	Orquestração dos jobs Pentaho (Staging → Remessa Diária), com retentativa automática em caso de erro
monitoramento_schema.sql	Schema PostgreSQL de log de execução e estatísticas agregadas para painel
Modelo de governança relacionado

O rastreamento de cadeia e a fricção deliberada aqui descritos se apoiam no modelo GSD-ISD (Governança da Simbiose Decisória / Índice de Simbiose Decisória), com demonstração interativa disponível em ericlopesmello.vercel.app.

Autor

Eric Lopes Mello — servidor do TRT-2, pesquisador em governança algorítmica e auditabilidade de IA no Poder Judiciário. Lattes: lattes.cnpq.br/4067922909268264

Licença

Conteúdo de acesso livre e gratuito.
