# 📱 Android na Prática — 10 Projetos com Kotlin e Jetpack Compose

> Uma trilha prática de desenvolvimento Android, do primeiro componente visual a aplicativos com persistência de dados, APIs e arquitetura MVVM.

![Kotlin](https://img.shields.io/badge/Linguagem-Kotlin-7F52FF?logo=kotlin&logoColor=white)
![Android Studio](https://img.shields.io/badge/IDE-Android%20Studio-3DDC84?logo=androidstudio&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?logo=jetpackcompose&logoColor=white)
![Projetos](https://img.shields.io/badge/Projetos-10-222222)

## 🎯 Objetivo

Este repositório foi pensado para estudantes e desenvolvedores que desejam aprender **Kotlin**, **Android Studio** e **Jetpack Compose** construindo dez aplicativos progressivamente mais completos.

Ao final da trilha, você terá praticado:

- Componentes declarativos com `@Composable`, `Text`, `Button`, `Column`, `Row` e `LazyColumn`.
- Gerenciamento de estado com `remember`, `rememberSaveable` e `ViewModel`.
- Formulários, validação e tratamento de eventos.
- Navegação entre telas com Navigation Compose.
- Persistência local com Room e DataStore, quando apropriado.
- Consumo de APIs REST com Retrofit, corrotinas e Kotlin Flow.
- Material Design 3, acessibilidade, testes e organização de código.

> **Status:** este README apresenta o **roteiro dos projetos**. A existência das pastas e a implementação de cada aplicativo devem ser conferidas no repositório à medida que forem adicionadas. O texto não pressupõe que todos os códigos já estejam prontos.

## 🧰 Pré-requisitos

- Android Studio com suporte a projetos Kotlin e Jetpack Compose.
- Android SDK e emulador configurados, ou um dispositivo Android para testes.
- Conhecimentos básicos de lógica de programação e Kotlin.
- Acesso à internet para sincronizar dependências e testar o projeto de API.

**Como iniciar cada aplicativo:** no Android Studio, selecione **New Project → Empty Activity**, escolha **Kotlin** e confirme que o projeto usa **Jetpack Compose**. Utilize as versões de SDK, Gradle e bibliotecas compatíveis sugeridas pelo assistente do Android Studio. Para dependências do Compose, prefira a **Compose BOM** e o plugin do compilador Compose conforme a documentação oficial.

## 🗂️ Catálogo dos 10 projetos

| # | Projeto | Nível | Conteúdos principais |
|---|---|---|---|
| 01 | Cartão de Visita Digital | 🟢 Iniciante | `Text`, `Image`, `Column`, `Row`, `Modifier` |
| 02 | Calculadora Interativa | 🟢 Iniciante | `Button`, estado, eventos e funções |
| 03 | Conversor de Temperatura | 🟢 Iniciante | `TextField`, validação e cálculos |
| 04 | Quiz Educacional | 🟢 Iniciante | `RadioButton`, listas, pontuação e estado |
| 05 | Temporizador Pomodoro | 🟡 Intermediário | Efeitos, corrotinas e ciclo de vida |
| 06 | Lista de Tarefas | 🟡 Intermediário | CRUD, Room, Flow e MVVM |
| 07 | Controle de Estoque | 🟡 Intermediário | Formulários, Room, filtros e relatórios |
| 08 | Previsão do Tempo | 🟡 Intermediário | HTTP, Retrofit, JSON e estados de tela |
| 09 | Controle Financeiro | 🔴 Avançado | Room, MVVM, gráficos e agregações |
| 10 | Corretor de Provas | 🔴 Avançado | Modelagem de avaliações, correção e histórico |

---

## 01 — 💼 Cartão de Visita Digital

**Objetivo:** criar um cartão de apresentação pessoal responsivo usando exclusivamente componentes Compose.

**Funcionalidades obrigatórias:**
- [ ] Mostrar foto ou avatar, nome, ocupação e breve descrição.
- [ ] Exibir contatos organizados com ícones.
- [ ] Disponibilizar botão para abrir e-mail ou perfil profissional.
- [ ] Aplicar cores, tipografia e espaçamentos consistentes.

**Você vai praticar:** `@Composable`, `Surface`, `Column`, `Row`, `Image`, `Text`, `Icon`, `Button` e `Modifier`.

**Desafio extra:** alternar entre tema claro e escuro.

**Critério de conclusão:** interface legível em um celular pequeno e um maior, sem corte de conteúdo.

**Pasta sugerida:** `01-cartao-visita/`

## 02 — 🧮 Calculadora Interativa

**Objetivo:** criar uma calculadora capaz de realizar operações aritméticas básicas.

**Funcionalidades obrigatórias:**
- [ ] Exibir visor numérico e teclado de operações.
- [ ] Realizar adição, subtração, multiplicação e divisão.
- [ ] Limpar o visor e permitir correção da entrada.
- [ ] Tratar divisão por zero e operações inválidas sem fechar o app.

**Você vai praticar:** `Button`, `LazyVerticalGrid` (opcional), `rememberSaveable`, eventos de clique e lógica com funções Kotlin.

**Desafio extra:** registrar um histórico das últimas operações.

**Critério de conclusão:** cálculos corretos, inclusive com números decimais e entradas inválidas.

**Pasta sugerida:** `02-calculadora/`

## 03 — 🌡️ Conversor de Temperatura

**Objetivo:** converter valores entre Celsius, Fahrenheit e Kelvin.

**Funcionalidades obrigatórias:**
- [ ] Receber temperatura em um campo de texto.
- [ ] Selecionar unidade de origem e destino.
- [ ] Atualizar o resultado da conversão.
- [ ] Informar erros de entrada e impedir valores abaixo do zero absoluto.

**Você vai praticar:** `OutlinedTextField`, `DropdownMenu`, `rememberSaveable`, funções matemáticas e validação de formulários.

**Desafio extra:** histórico de conversões e botão para trocar as unidades.

**Critério de conclusão:** resultado consistente nas três escalas, com arredondamento apenas na apresentação.

**Pasta sugerida:** `03-conversor-temperatura/`

## 04 — 🧠 Quiz Educacional

**Objetivo:** desenvolver um jogo de perguntas e respostas com pontuação final.

**Funcionalidades obrigatórias:**
- [ ] Apresentar questões de múltipla escolha.
- [ ] Permitir a seleção de uma alternativa por pergunta.
- [ ] Avançar entre questões e indicar progresso.
- [ ] Exibir nota, acertos e erros ao finalizar.

**Você vai praticar:** `RadioButton`, estruturas de dados (`data class`), listas, condicionais, gerenciamento de estado e navegação simples.

**Desafio extra:** adicionar categorias, cronômetro e embaralhamento de perguntas.

**Critério de conclusão:** não permitir múltiplas respostas na mesma pergunta e calcular corretamente o resultado.

**Pasta sugerida:** `04-quiz-educacional/`

## 05 — ⏱️ Temporizador Pomodoro

**Objetivo:** criar um temporizador para ciclos de estudo e descanso.

**Funcionalidades obrigatórias:**
- [ ] Iniciar, pausar, continuar e reiniciar uma contagem regressiva.
- [ ] Alternar entre sessão de foco e intervalo.
- [ ] Mostrar tempo restante e progresso visual.
- [ ] Preservar estado básico durante recomposições e mudanças de orientação.

**Você vai praticar:** `CircularProgressIndicator`, `LaunchedEffect`, corrotinas, `ViewModel` e noções de ciclo de vida.

**Desafio extra:** configurações persistidas com DataStore e notificações ao término.

**Critério de conclusão:** a contagem não deve acelerar por recomposição nem criar temporizadores duplicados.

**Pasta sugerida:** `05-pomodoro/`

## 06 — ✅ Lista de Tarefas

**Objetivo:** implementar uma lista de tarefas com armazenamento local.

**Funcionalidades obrigatórias:**
- [ ] Cadastrar uma tarefa com título e descrição opcional.
- [ ] Listar tarefas em `LazyColumn`.
- [ ] Editar, concluir e excluir tarefas.
- [ ] Persistir alterações após fechar e reabrir o aplicativo.

**Você vai praticar:** Room (`Entity`, `Dao`, `Database`), `ViewModel`, `Flow`, `collectAsStateWithLifecycle` e organização MVVM.

**Desafio extra:** adicionar prioridade, data de vencimento e filtros.

**Critério de conclusão:** fluxo completo de criar, consultar, atualizar e excluir (CRUD), com persistência verificada.

**Pasta sugerida:** `06-lista-tarefas/`

## 07 — 📦 Controle de Estoque

**Objetivo:** desenvolver um cadastro local de produtos e movimentações de quantidade.

**Funcionalidades obrigatórias:**
- [ ] Cadastrar nome, categoria, preço e quantidade em estoque.
- [ ] Editar e remover produtos, com confirmação.
- [ ] Registrar entradas e saídas de unidades.
- [ ] Pesquisar produtos e destacar itens abaixo do estoque mínimo.

**Você vai praticar:** formulários Compose, validação, Room, MVVM, filtros, estados de interface e cálculos monetários com tipos adequados.

**Desafio extra:** relatório de movimentações e exportação CSV.

**Critério de conclusão:** impedir estoque negativo e manter as quantidades consistentes após reiniciar o aplicativo.

**Pasta sugerida:** `07-controle-estoque/`

## 08 — ☁️ Previsão do Tempo

**Objetivo:** consultar dados meteorológicos de uma API e apresentar os resultados em uma tela Compose.

**Funcionalidades obrigatórias:**
- [ ] Pesquisar uma cidade pelo nome.
- [ ] Consumir um serviço de previsão do tempo com Retrofit.
- [ ] Exibir temperatura, condição e informações disponíveis na resposta da API.
- [ ] Apresentar estados de carregamento, sucesso, falha e ausência de resultados.

**Você vai praticar:** Retrofit, desserialização JSON, permissões de internet, `suspend`, `ViewModel` e arquitetura com repositório.

**Desafio extra:** armazenar a última consulta em cache e permitir atualização manual.

**Critério de conclusão:** a tela não deve travar durante requisições e erros de rede devem ser compreensíveis.

**Observação:** escolha uma API meteorológica com condições de uso adequadas. Não coloque chaves privadas no repositório.

**Pasta sugerida:** `08-previsao-tempo/`

## 09 — 💰 Controle Financeiro Pessoal

**Objetivo:** registrar receitas e despesas e gerar um resumo financeiro local.

**Funcionalidades obrigatórias:**
- [ ] Cadastrar receitas e despesas com valor, categoria e data.
- [ ] Listar, editar e excluir transações.
- [ ] Filtrar lançamentos por período e categoria.
- [ ] Calcular receitas, despesas e saldo do período.
- [ ] Apresentar um painel com resumo e gráfico simples.

**Você vai praticar:** Room, Flow, MVVM, agregações, componentes gráficos e tratamento correto de valores monetários.

**Desafio extra:** orçamento por categoria e exportação dos próprios dados.

**Critério de conclusão:** totais coerentes com os registros armazenados e atualização automática da interface.

**Pasta sugerida:** `09-controle-financeiro/`

## 10 — 📝 Corretor de Provas

**Objetivo:** construir um aplicativo para cadastrar gabaritos, corrigir respostas e organizar resultados de avaliações.

**Funcionalidades obrigatórias:**
- [ ] Criar avaliações com título, turma e quantidade de questões.
- [ ] Cadastrar gabaritos de alternativas (A, B, C, D, E).
- [ ] Inserir identificação do aluno e respostas marcadas.
- [ ] Calcular acertos, erros e nota com base em uma regra definida.
- [ ] Consultar histórico de correções e resultados por turma.

**Você vai praticar:** modelagem de entidades relacionadas, Room, `Navigation Compose`, ViewModel, formulários dinâmicos, validação e relatórios.

**Desafio extra:** ler cartão-resposta por câmera com uma etapa separada de reconhecimento de marcações e revisão manual, antes de salvar a nota.

**Critério de conclusão:** cada nota deve ser reproduzível a partir do gabarito e das respostas armazenadas; dados de alunos precisam de proteção adequada.

**Pasta sugerida:** `10-corretor-provas/`

---

## 🧱 Estrutura sugerida do repositório

À medida que os projetos forem implementados, organize-os desta forma:

```text
android-kotlin-compose-10-projetos/
├── README.md
├── 01-cartao-visita/
├── 02-calculadora/
├── 03-conversor-temperatura/
├── 04-quiz-educacional/
├── 05-pomodoro/
├── 06-lista-tarefas/
├── 07-controle-estoque/
├── 08-previsao-tempo/
├── 09-controle-financeiro/
└── 10-corretor-provas/
```

Cada pasta pode conter seu próprio projeto Android Studio, documentação e capturas de tela. **Não são dez módulos obrigatórios de um único aplicativo:** são dez aplicativos independentes.

Uma organização interna recomendada para os projetos intermediários e avançados é:

```text
app/src/main/java/com/exemplo/projeto/
├── data/           # entidades, DAOs, API e repositórios
├── domain/         # modelos e regras de negócio, se necessário
├── ui/
│   ├── screens/    # telas @Composable
│   ├── components/ # componentes reutilizáveis
│   └── theme/      # cores, fontes e tema
└── MainActivity.kt
```

## ▶️ Como executar um projeto

1. Instale o [Android Studio](https://developer.android.com/studio).
2. Baixe o repositório pelo botão **Code → Download ZIP** ou use `git clone URL_DO_REPOSITORIO`.
3. No Android Studio, selecione **Open** e abra a **pasta do aplicativo** desejado, quando ela já estiver implementada.
4. Aguarde o **Gradle Sync** concluir e instale os SDKs sugeridos, se necessário.
5. Configure um emulador Android ou conecte um dispositivo com depuração USB habilitada.
6. Clique em **Run ▶** para compilar e executar.

> Para projetos ainda não adicionados, crie um novo aplicativo **Empty Activity** com Kotlin e Jetpack Compose e salve-o na pasta correspondente.

## 🧪 Padrão de entrega de cada projeto

- [ ] Código-fonte Kotlin organizado e compilando.
- [ ] Interface construída em Jetpack Compose, sem necessidade de layouts XML.
- [ ] Funcionalidades obrigatórias implementadas.
- [ ] Validação de entradas e tratamento de erros.
- [ ] Pelo menos uma captura de tela no README da pasta.
- [ ] Instruções de execução e descrição das decisões técnicas.
- [ ] Testes básicos para a lógica principal, conforme a complexidade do projeto.
- [ ] Nenhuma senha, token ou chave privada versionada.

## 🎓 Sugestão de avaliação acadêmica

| Critério | Peso |
|---|---:|
| Funcionalidades obrigatórias e correção da lógica | 35% |
| Interface, usabilidade e acessibilidade | 20% |
| Organização do código e uso adequado de Compose | 20% |
| Tratamento de erros e testes | 15% |
| Documentação e apresentação | 10% |
| **Total** | **100%** |

## 🔗 Referências oficiais

- [Kotlin — documentação](https://kotlinlang.org/docs/home.html)
- [Android Developers — cursos com Compose](https://developer.android.com/courses/android-basics-compose/course)
- [Jetpack Compose — visão geral](https://developer.android.com/develop/ui/compose)
- [Configurar Compose e suas dependências](https://developer.android.com/develop/ui/compose/setup-compose-dependencies-and-compiler)
- [Arquitetura de aplicativos Android](https://developer.android.com/topic/architecture)
- [Room](https://developer.android.com/training/data-storage/room)

## 🤝 Como contribuir

Contribuições com melhorias, correções, documentação ou novos desafios são bem-vindas. Antes de abrir um pull request, descreva as alterações e verifique se o projeto afetado compila e executa.

## 📄 Licença

**A definir.** Antes de reutilizar ou distribuir o código de terceiros, verifique as licenças aplicáveis. Se quiser permitir reutilização formal deste material, adicione ao repositório um arquivo `LICENSE` com a licença escolhida.

---

**Bons estudos!** 🚀 Desenvolva os projetos em sequência, experimente variações e registre sua evolução no GitHub.
