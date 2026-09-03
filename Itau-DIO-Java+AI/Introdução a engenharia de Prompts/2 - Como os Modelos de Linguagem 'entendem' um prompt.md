
- Os modelos LLM calculam probabilidade com base nos padrões aprendidos durante o treinamento;
- Arquitetura Transformer permite que os modelos compreendam de forma mais eficaz os prompts;
- A Arquitetura Transformer utiliza mecanismos de atenção para processar palavras em sequência considerando o contexto de cada palavra em relação a todas as outras do texto e não de forma linear;

### Como os modelos de linguagem processam os prompts

- Ao fornecer um prompt para o modelo, o mesmo converte o texto em uma sequencia de tokens;
- Tokens - são unidades básicas, que podem ser: palavras, partes de palavras ou até mesmo caracteres.
- A sequencia de tokens é processada pelas camadas de atenção e por outras transformações até gerar a resposta;
- Ferramenta Tokenizer 
-  Após o processo de tokenização, os tokens são convertidos em embeddings
- Embeddings: São representações vetoriais que capturam o seu significado
-  Após isso os embeddings passam por camadas de redes neurais com transformadores e o modelo aplica estas operações para poder entender o contexto;
- Então o modelo gera uma distribuição de probabilidades para tentar prever o próximo token;
- O processo de tentar prever o token seguinte é repetido até gerar a sequencia;

### Como os modelos de linguagem 'lembram' do que foi dito

- O modelo dentro da interação consegue manter o contexto do que foi dito por meio da janela de contexto;
- Janela de Contexto é o limite de tokens que o modelo consegue processar simultaneamente;
- Cada modelo possui uma janela de contexto diferente;
- Quando este limite é atingido, os tokens mais antigos são descartados para dar lugar aos mais novos;

### Elementos essenciais para construir um bom prompt

- Instrução clara - Tarefa específica que você quer que o modelo execute;
- Contexto Adequado - Informações que ajudam o modelo a entender a tarefa que tem que executar;
- Exemplos - Vão ajudar a orientar o modelo quanto ao formato ou estilo em relação a tarefa a ser executada;
- Dados de entrada - são informações ou problema específico que você deseja que o modelo processe ou resolva; 
- Formato de saída - Aqui você consegue especificar qual o formato que o modelo vai retornar a saída;