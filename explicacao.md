### Classe Abstrata `Pessoa`

- **Propósito:** Serve como base para outras classes representando pessoas, como `Motorista` e `Passageiro`. Ela é abstrata, significando que não pode ser instanciada diretamente, apenas herdada.
- **Propriedades Protegidas:** `id`, `nome`, `cpf`. Esses atributos são protegidos, significando que só podem ser acessados dentro da classe e suas subclasses.
- **Construtor:** Inicializa as propriedades da classe com valores fornecidos.
- **Métodos de Acesso (Getters):** Permite a leitura dos valores das propriedades `id`, `nome` e `cpf`.

### Classe `Motorista`

- **Herança:** Extende a classe `Pessoa`, herdando suas propriedades e métodos.
- **Propriedades Adicionais:** `carteiraMotorista` e `salario`.
- **Métodos Específicos:** Incluem `iniciarViagem()`, `finalizarViagem()`, `relatarProblema()` e `visualizarRota()`, cada um executando uma ação específica do motorista, como iniciar ou finalizar uma viagem, e imprimir mensagens relacionadas.

### Classe `Passageiro`

- **Herança:** Também extende a classe `Pessoa`.
- **Propriedade Adicional:** `bilhetesComprados`, um array para armazenar os bilhetes comprados pelo passageiro.
- **Métodos Específicos:** `comprarBilhete()`, que cria e armazena um novo bilhete no array de bilhetes, e `cancelarBilhete()`, que procura um bilhete pelo ID e o remove do array se encontrado.

### Classe `Onibus`

- **Propriedades:** `id`, `modelo`, `capacidade`, `estado`. Descrevem características básicas do ônibus.
- **Métodos:** `alterarEstado()` para mudar o estado do ônibus (e.g., de "disponível" para "em manutenção") e getters para `id` e `estado`.

### Classe `Rota`

- **Propriedades:** `id`, `nome`, `origem`, `destino`, `horarios`, `onibusAlocados`. Armazena informações sobre cada rota, incluindo quais ônibus estão alocados para ela.
- **Métodos:** Incluem adicionar/remover ônibus da rota e adicionar/remover horários da rota.

### Classe `Bilhete`

- **Propriedades:** Identifica cada bilhete vendido, incluindo `id`, `rota`, `horario`, `passageiroId`, `estado`.
- **Métodos:** `cancelar()`, que muda o estado do bilhete para "cancelado".

### Classe `CompaniaDeOnibus`

- **Propriedades:** `nome`, `cnpj`, arrays para armazenar `onibus`, `rotas`, e `motoristas`.
- **Métodos:** Métodos para adicionar e remover ônibus, rotas e motoristas da companhia.

### Exemplo de Utilização das Classes

As últimas linhas do código demonstram como utilizar essas classes para criar objetos representando motoristas, passageiros, ônibus, rotas, e como adicionar esses elementos à companhia de ônibus, comprar e cancelar bilhetes, e iniciar/finalizar viagens.

### Pontos para Destacar na Apresentação

- **Orientação a Objetos:** O código é um bom exemplo do uso de conceitos de orientação a objetos, como herança, encapsulamento, e polimorfismo (através de métodos sobrescritos e classes abstratas).
- **Reutilização e Organização:** A estruturação em classes permite a reutilização de código (por exemplo, `Pessoa` como classe base) e orgEste código é um exemplo prático de um sistema de gerenciamento de transporte coletivo usando PHP orientado a objetos. Vou detalhar cada parte para te ajudar a entender e explicar durante sua apresentação:

### Classe Abstrata `Pessoa`

- **Propósito:** Serve como base para outras classes representando pessoas, como `Motorista` e `Passageiro`. Ela é abstrata, significando que não pode ser instanciada diretamente, apenas herdada.
- **Propriedades Protegidas:** `id`, `nome`, `cpf`. Esses atributos são protegidos, significando que só podem ser acessados dentro da classe e suas subclasses.
- **Construtor:** Inicializa as propriedades da classe com valores fornecidos.
- **Métodos de Acesso (Getters):** Permite a leitura dos valores das propriedades `id`, `nome` e `cpf`.

### Classe `Motorista`

- **Herança:** Extende a classe `Pessoa`, herdando suas propriedades e métodos.
- **Propriedades Adicionais:** `carteiraMotorista` e `salario`.
- **Métodos Específicos:** Incluem `iniciarViagem()`, `finalizarViagem()`, `relatarProblema()` e `visualizarRota()`, cada um executando uma ação específica do motorista, como iniciar ou finalizar uma viagem, e imprimir mensagens relacionadas.

### Classe `Passageiro`

- **Herança:** Também extende a classe `Pessoa`.
- **Propriedade Adicional:** `bilhetesComprados`, um array para armazenar os bilhetes comprados pelo passageiro.
- **Métodos Específicos:** `comprarBilhete()`, que cria e armazena um novo bilhete no array de bilhetes, e `cancelarBilhete()`, que procura um bilhete pelo ID e o remove do array se encontrado.

### Classe `Onibus`

- **Propriedades:** `id`, `modelo`, `capacidade`, `estado`. Descrevem características básicas do ônibus.
- **Métodos:** `alterarEstado()` para mudar o estado do ônibus (e.g., de "disponível" para "em manutenção") e getters para `id` e `estado`.

### Classe `Rota`

- **Propriedades:** `id`, `nome`, `origem`, `destino`, `horarios`, `onibusAlocados`. Armazena informações sobre cada rota, incluindo quais ônibus estão alocados para ela.
- **Métodos:** Incluem adicionar/remover ônibus da rota e adicionar/remover horários da rota.

### Classe `Bilhete`

- **Propriedades:** Identifica cada bilhete vendido, incluindo `id`, `rota`, `horario`, `passageiroId`, `estado`.
- **Métodos:** `cancelar()`, que muda o estado do bilhete para "cancelado".

### Classe `CompaniaDeOnibus`

- **Propriedades:** `nome`, `cnpj`, arrays para armazenar `onibus`, `rotas`, e `motoristas`.
- **Métodos:** Métodos para adicionar e remover ônibus, rotas e motoristas da companhia.

### Exemplo de Utilização das Classes

As últimas linhas do código demonstram como utilizar essas classes para criar objetos representando motoristas, passageiros, ônibus, rotas, e como adicionar esses elementos à companhia de ônibus, comprar e cancelar bilhetes, e iniciar/finalizar viagens.

### Pontos para Destacar na Apresentação

- **Orientação a Objetos:** O código é um bom exemplo do uso de conceitos de orientação a objetos, como herança, encapsulamento, e polimorfismo (através de métodos sobrescritos e classes abstratas).
- **Reutilização e Organização:** A estruturação em classes permite a reutilização de código (por exemplo, `Pessoa` como classe base) e organização lógica do sistema.
- **Extensibilidade:** O design permite a fácil adição de novas funcionalidades, como novos tipos de pessoas (ex.: inspetores), novos atributos para as rotas ou ônibus, etc.

Estudando esses pontos, você estará bem preparado para explicar seu código e responder a perguntas durante a apresentanização lógica do sistema.
- **Extensibilidade:** O design permite a fácil adição de novas funcionalidades, como novos tipos de pessoas (ex.: inspetores), novos atributos para as rotas ou ônibus, etc.

Estudando esses pontos, você estará bem preparado para explicar seu código e responder a perguntas durante a apresent