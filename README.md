# Verificando erro na execução de uma operação

Se sua operação foi feita corretamente com mensageria, poderá acessar o erro pelo catálogo.
### Acessando o Catálogo Corporativo
- Efetue o login na intranet;
- Selecione a opção Catálogo no canto superior esquerdo;
- Mais ou menos no meio da pagina, na parte superior, selecione a opção tecnologia(dentro do icone com 9 quadradinhos);
- Na coluna da esquerda, tem um ícone em forma de chave inglesa. Aponte o ponteiro do mouse sobre ela;
- Localize a opção "Catálogo" e selecione a opção "Corporativo de TI";

### Encontrando o erro na mensageria
- Dentro da página do Catálogo, no menu superior, selecione "Mensageria";
- Listar ocorrências por módulo;
- Na página "Listar ocorrências por módulo mainframe", preencha:
    - o nome do módulo;
    - a data da ocorrência do erro;
    - hora inicial e hora final;
    - ambiente(muito importante selecionar corretamente);
- Clique no ícone com uma apulheta no meio de um quadrado para o sistema listar os erros.

# Cadastramento de operação no Catálogo

Como efetuar o cadastro de uma operação no catálogo corporativo?
<br>
Veja no passo a passo abaixo a sequência básica:

### Acessando o Catálogo Corporativo
- Efetue o login na intranet;
- Selecione a opção Catálogo no canto superior esquerdo;
- Mais ou menos no meio da pagina, na parte superior, selecione a opção tecnologia(dentro do icone com 9 quadradinhos);
- Na coluna da esquerda, tem um ícone em forma de chave inglesa. Aponte o ponteiro do mouse sobre ela;
- Localize a opção "Catálogo" e selecione a opção "Corporativo de TI";

### Cadastrando a nova operação
- Na página de Catálogo Corporativo de TI, na coluna da esquerda em "Acesso rápido", selecione "Criar nova operação - serviço genérico";
- Localize e selecione a opção de "Adicionar operação";
- Abrirá uma pagina para cadastro de:
    - Nome: nome da operação com todas as palavras em maiúsculo e válidas no dicionário de termos do AD(sem caracteres especiais);
    - Descrição: breve descrição da operação que está sendo cadastrada;
    - Book de entrada: área de requisição da operação. Os nome dos campos devem respeitar as abreviaturas do dicionário de termos do AD
      e não se podem repetir campos com mesmo nome. Ex.: FILLER(mesmo porquê não consta no dicionário de termos do AD);
    - Prefixo a suprimir: parte do nome do campo que não deve ser validado. 
      Ex. XP123-CD-PRF-DEPE  termo que deve ser suprimido: XP123
    - Book de saída: área de resposta da operação. Deve respeitar a mesma regra do book de entrada;
    - Prefixo a suprimir: parte do nome do campo que não deve ser validado. Idem Book de entrada;
    - Escolha a operação padrão: normalmente "Mainframe CICS Sincrona-Container"
    - Sigla: sigla do sistema. Ex. DJO
    - Clique em importar book.
- Caso ocorra algum erro, este deverá ser ajustado;
- Se der tudo certo uma página será aberta com vários ícones na parte superior, entre eles um representando "Validação". Uma prancheta com um "V" verde dentro. Escolha este;
- Na página que será aberta selecione a opção de validação novamente;
- Na área de "Dados do contrato", selecione "Aplicar nomes sugeridos válidos";
- O catálogo vai validar cada uma das abreviaturas substituindo por nomes válidos. as abreviaturas não válidas não serão substituídas;
- Os campos que ficarem com X vermelho deverão ser corrigidos. Quando tudo estiver verdinho, clique em Salvar e depois em voltar;
- Na coluna da direita selecione a aba "ventos";
- Clique na ampulheta(detalhar evento da operação);
- Na parte superior esquerda está escrito: Evento de transação da operação, selecione a opção de edição(papel com um lápis);
- Na coluna da direita, corra a barra para baixo até aparecer Provedor mainframe CICS;
- Em container de requisição coloque o nome do programa que efetuará a operação seguido de RQSC. Ex.: DJOSP243-RQSC;
- Em container de resposta coloque o nome do programa que efetuará a operação seguido de RPST. Ex.: DJOSP243-RPST;
- Em módulo, somente o nome do programa;
- Em transação roteamento, coloque a sigla do sistema seguido de "$". Ex.: DJO$;
- Salve e retorne;
- Na coluna da esquerda, na parte do meio, tem uma opção chamada ações. Selecione o ícone azul com a descrição: publicar operação no ambiente de desenvolvimento;
- Inclua uma motivação/observação e clique em "transferir desenvolvimento";
- Se tudo der certo, a operação será publicada.
