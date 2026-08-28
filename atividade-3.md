# Atividade Avaliativa 3, Modelo Relacional e Mapeamento do MER para o Modelo Relacional

**Instruções:** cada questão vale 5,0 pontos. Marque a alternativa correta com um `x` dentro do checkbox (`- [x]`) e escreva sua justificativa no campo indicado.

---

**1.** Em uma tabela do modelo relacional, é preciso garantir que cada linha (registro) possa ser identificada de forma única, sem ambiguidade, mesmo que duas linhas tenham valores parecidos em várias colunas. Qual mecanismo do modelo relacional resolve isso?

- [ ] a) Chave estrangeira
- [x] b) Chave primária, pois identifica de forma única cada linha (registro) de uma tabela do modelo relacional
- [ ] c) Índice, pois é o único mecanismo do modelo relacional capaz de impedir que duas linhas fiquem iguais entre si
- [ ] d) Nenhum mecanismo é necessário
- [ ] e) Chave primária e chave estrangeira são a mesma coisa

**Justificativa:** A chave primária é um jeito de identificar cada registro da tabela de forma única, como dois clientes por exemplo poderiam ter o mesmo nome e terem nascido até mesmo no mesmo lugar, mas por conta de ter um ID, um identificador, daria para saber que são clientes diferentes.

**2.** Ao mapear para o modelo relacional um relacionamento muitos-para-muitos (N:N) do Modelo Entidade-Relacionamento (ex.: "Pedido" e "Produto"), qual é a estratégia correta?

- [ ] a) Relacionamentos N:N não podem ser representados no modelo relacional, sendo necessário redesenhar o MER original
- [ ] b) Duplicar a entidade em duas tabelas idênticas
- [x] c) Criar uma tabela associativa com as chaves estrangeiras das duas entidades
- [ ] d) Vira uma única coluna extra na tabela principal
- [ ] e) Relacionamentos N:N são sempre convertidos em um relacionamento um-para-um (1:1) entre as duas entidades envolvidas

**Justificativa:** Ao criar uma tabela associativa com as chaves estrangeiras das duas entidades seria possível identificar quais produtos teriam em um mesmo pedido (através do ID dos produtos) e também em quais pedidos um certo produto está (através do ID dos pedidos).
