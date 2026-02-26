Modelagem de Casos de Uso

Atores:
Coordenador;
Professor;
Estudante EJA;

Caso de Uso 1 – Enviar Material Didático
Ator: Professor
Pré-condição: Professor autenticado
Fluxo Principal:
Seleciona turma;
Anexa arquivo;
Define descrição;
Publica.
Fluxo Alternativo:
Arquivo inválido → mensagem de erro
Pós-condição: Material disponível aos estudantes

Caso de Uso 2 – Enviar Avaliação Online
Ator: Professor

Caso de Uso 3 – Realizar Avaliação Online
Ator: Estudante
Pré-condição: Avaliação disponível
Fluxo Principal:
Acessa avaliação;
Responde questões;
Submete respostas;
Recebe confirmação.
Fluxo Alternativo:
Tempo expirado → submissão automática
Pós-condição: Respostas registradas

Caso de Uso 4 – Enviar Feedback Individual
Ator: Professor
Fluxo Principal:
Acessa desempenho do aluno
Registra comentário
Envia feedback
Pós-condição: Estudante recebe notificação

Caso de Uso 5 – Enviar Atividade
Ator: Professor

Caso de Uso 6 – Realizar Atividade
Ator: Estudante

Caso de Uso 7 - Enviar avisos e informes
Ator: Coordenador
Fluxo Principal:
Acessa o aviso/informe
Identifica a turma
Escreve o título
Registra a mensagem
Envia a mensagem
Pós-condição: Professor e Estudante recebem a mensagem

Fluxo de Navegação
Login
→ Painel do Coordenador, Professor ou Estudante
→ Materiais
→ Avaliações
→ Desempenho
→ Aviso/Informe
Protótipo de Interface (Inicial)
Estrutura (sugerida):
Dashboard
Menu lateral:
Presença
Materiais
Avaliações
Desempenho
Aviso/Informe

Interface minimalista, com foco em clareza e acessibilidade.

Modelo de Dados Inicial
Entidades principais:
Usuário (id, nome, perfil, email)
Turma (id, nome, ano)
Material (id, título, arquivo, data)
Avaliação (id, tipo, data)
Resposta (id, aluno_id, nota)
Presença (aluno_id, data, status)
Avisos/Informes (turma-id, título, mensagem, data)

Integração com Projetos Integradores
Projeto Integrador I
Informática e letramento digital
Projeto Integrador II
NR-10 e terminologia técnica de segurança elétrica
Projeto Integrador III
Crise hídrica e geração de energia

O sistema incorporará vocabulário técnico contextualizado a essas temáticas e com versão em língua inglesa.

Foco Especializado em ESP (English for Specific Purposes)
O sistema integra:
Glossário técnico bilíngue
Atividades com textos técnicos
Simulações linguísticas de contexto profissional
Avaliações com terminologia da área de eletrotécnica com foco nos projetos integradores

Critérios de Avaliação e Validação
Implementação completa dos requisitos
Testes por meio do uso do sistema com turma piloto nas aulas do Projeto Integrador I e de Inglês Instrumental 
Coleta de feedback qualitativo por meio da observação do pesquisado-participante e notas de campo
Análise de usabilidade por meio da observação do pesquisado-participante e notas de campo
Relatório técnico-científico parcial e final.

Potencial Científico
O sistema funcionará como ambiente controlado para:
Testar metodologias ESP;
Avaliar impacto pedagógico;
Produzir dados para publicação científica;
Propor melhorias futuras ao sistema institucional (como o Sistema Unificado de Administração Pública - SUAP)

Estrutura do Repositório
pibic-ifg-esp-learning-eletrotecnica-system/
├── assets\
│   ├── imagens\
│   ├── videos\
│   └── projeto-de-Pesquisa-PIBIC-desenvolvimento-sistetma-digital.pdf
│
├── docs\
│   ├── casos-de-uso.md
│   ├── cronograma.md
│   └── ers-srs.md   
│   ├── prd-modelo.md
│   └── prd-versao-orientando.md
│   └── referencial-teorico.md
├── src/
│   ├── frontend/
│        └── css\
│             └── style.css
│        └── html\
│             └── index.html
│        └── js\
│             └── script.js
└── .gitignore
└── LICENSE
└── README.md
