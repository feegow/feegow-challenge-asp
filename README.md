# Feegow Challenge

Esse é um case focado em design de código, e conhecimento da linguagem e seus principais recursos. O objetivo é avaliar sua experiênica em escrever código de fácil manutenção, baixo acoplamento, e alta coesão.


## Apresentação do problema

A clínica _Exemplo_ precisa exibir a listagem de seus médicos separados por especialidade em seu site para que seus pacientes tenham acesso. Essa clínica utiliza o Feegow que possui uma api que fornece o suporte necessário para isso. 
Link da documentação: https://api.feegow.com.br/api/documentation 

  1- A tela inicial deve ser um SELECT contendo a listagem de todas as especialidades que a clínica trabalha (método na documentação: ``GET /specialties/list``). 
  
  ![Exemplo do SELECT](https://image.prntscr.com/image/krKCLaZGT1O3rf4h4ETLow.png)
  
  
  2- Quando o usuário escolhe uma especialidade, é executado um AJAX para buscar os profissionais que possuem aquela especialidade e exibido em tela (método na documentação: ``GET /professional/list``). 

  ![Exemplo do SELECT](https://image.prntscr.com/image/v4cm7l99TOuvcyhHuIgaJw.png)

  3- Quando o usuário clicar em "AGENDAR", será exibido um formulário que o usuário irá preencher e clicar em "ENVIAR".
  
  ![Exemplo do SELECT](https://image.prntscr.com/image/w34r0YIUQsmlJcq7DcaIQA.png)
  
  4- Quando o usuário enviar, deverá enviar o formulário por AJAX e salvar todas as informações em um banco de dados relacional contendo: **specialty_id, professional_id, name, cpf, source_id (GET /patient/list-sources), birthdate e date_time**.
      
  Obs: A listagem do campo "Como conheceu" deve vir da api (método ``GET /patient/list-sources`` )
  
  5- Após salvar as informações exibir uma informação ao usuário que os dados foram salvos.


## Tecnologias usadas

Os pré-requisitos para a aplicação:

- Use o ASP Classico como linguagem backend.
- Usar Bootstrap ou qualquer framework front-end de sua preferência.
- O banco de dados deve ser relacional (preferencia MySQL/POSTGRESQL).
- Documentação sucinta e explicativa de como levantar os ambientes necessários e executar seu código.

## Avaliação

Para nos enviar seu código, você poderá escolher as 3 opções abaixo:

- Fazer um fork desse repositório e nos mandar uma pull-request
- Dar acesso ao seu repositório no Github para _FeegowWelcomeTech_ .
- Enviar um git bundle do seu repositório para os e-mail welcome.tech@feegow.com.br.

Caso opte por fazer um Pull-Request, deixe ele explicativo apontando tudo que precisa ser feito para executar a sua aplicação (inclusive a versão dos sistemas operacionais e programas necessários). 

## Dicas

- Aproveite os recursos das ferramentas que você está usando. Diversifique e mostre que você domina cada uma delas.
- Tente escrever seu codigo o mais claro e limpo possível. Código deve ser legível assim como qualquer texto dissertativo.
- Se destaque mostrando algo interessante e surpreendente. Isso sempre fará diferença.

## Serão considerados diferenciais neste case

- Estruturação do Banco de Dados em sua melhor forma normal
- Validações dos dados no front-ent e no back-end
- Aplicação de Bootstrap (https://getbootstrap.com/) e jquery (https://jquery.com/), explorando seus recursos de forma otimizada no front-end
- Aplicação de regras de segurança na aplicação

Qualquer dúvida técnica, envie uma mensagem para welcome.tech@feegow.com.br.

Você terá 3 dias para fazer esse teste, a partir do recebimento deste desafio. Sucesso!
