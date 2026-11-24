# JurisPrep IA

**Projeto Integrador — Profissional de TI: Empregabilidade e Portfólio | Gran Faculdade**

## Objetivo
Protótipo LegalTech/EdTech para auxiliar a organização de apostilas jurídicas destinadas a concursos de Delegado de Polícia e Analista Judiciário. Une classificação de temas por aprendizado de máquina, controle editorial e revisão ativa. O projeto foi desenvolvido com auxílio de IA generativa para fins acadêmicos; o estudante deve compreender, testar e adaptar o código antes de apresentá-lo.

## Como executar
1. Baixe o repositório (Code > Download ZIP) e extraia os arquivos.
2. Abra `index.html` no navegador. Não precisa instalar dependências, criar chave de API ou acessar um servidor.
3. Use **Carregar exemplo**, confira a classificação, escolha a disciplina e clique em **Estruturar apostila**.
4. Exporte o Markdown ou o CSV de revisão. Para PDF, use **Imprimir / salvar PDF** e selecione Salvar como PDF na janela do navegador.

## Funcionalidades
- Classificação de texto por Naive Bayes multinomial, com suavização de Laplace e cinco classes.
- Treinamento local com 25 exemplos sintéticos; normalização de acentos, vocabulário e escores relativos.
- Seleção humana da disciplina, registro de fonte e data de conferência.
- Estrutura de apostila: conteúdo-base, lei seca, jurisprudência, objetiva, discursiva, peça, oral e revisão.
- Exportação Markdown, CSV de perguntas de revisão e impressão.

## Fluxo técnico
Entrada de texto → tokenização → Naive Bayes → sugestão de disciplina → revisão humana → estrutura e exportação.

## Limitações e ética
Não é um gerador de doutrina jurídica autônomo, não consulta fontes em tempo real, não valida URLs, legislação, julgados ou conteúdo jurídico. O pequeno corpus não foi validado em uma amostra representativa de provas reais. As lacunas são marcadas para preenchimento; os flashcards exigem revisão. A finalidade é educacional, não substitui orientação jurídica. O sistema roda no navegador sem enviar dados para serviços externos. Não inclua dados pessoais, processos sigilosos ou material de terceiros sem autorização. Os documentos pessoais de planejamento que inspiraram o projeto não fazem parte do repositório.

## Fontes para conferência manual
- Legislação: https://www.planalto.gov.br/
- Supremo Tribunal Federal: https://portal.stf.jus.br/
- Superior Tribunal de Justiça: https://www.stj.jus.br/

## Tecnologias
HTML5, CSS, JavaScript, aprendizado de máquina (Naive Bayes), Markdown e CSV.

## Testes
Com Node.js instalado, execute `node testes.cjs`. Os testes verificam exemplos de classificação, ausência de vocabulário conhecido, geração de estrutura e proteção de células CSV. São testes de comportamento, não prova de precisão jurídica ou estatística.

## Próximas evoluções
Banco de questões com metadados, análise de incidência por banca, integração com fontes oficiais e recuperação de documentos com citações verificáveis, mediante avaliação de qualidade.
