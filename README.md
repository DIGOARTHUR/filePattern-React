# Folder Structure - React

## Folder Structure




- `api`: diretório que contém todos os serviços que cuidam da comunicação entre o React (frontend) e a API (backend)
   - `services`: Aqui ficam as configurações de HTTP clientes, normalmente utilizando axios.
   - `auth`: aqui é feita todo o processo de autenticação. Caso a sua aplicação tenha um sistema de Login, terá que ser construído todo um contexto, todo um estado Global para que tenha, cuidadosamente,  controle como por exemplo: autorização de acesso a recursos da aplicação.
   
   


`assets`: Serve para armazenar imagens, ícones, audios, videos.



`componentes`: Componentes reutilizáveis da aplicação. Componentes que são unidades para sua aplicação, um button, um dropdown, um modal, um input etc.




 - `pages`: As pages são as páginas que usam vários componentes. É essa a página que o usuário vai ver.

   - `test`: aqui fica toda a estrutura para testes. É conveniente colocar junto aos arquivos de cada página para que corresponda aos mesmos.



`store`: este diretório inclui todos os estados globais do React que podem ser acessados a partir de qualquer componente do aplicativo. Podem ser usados state managers, context api, zustand, redux.

`types`: Armazena as tipagens de typescript (types e interfaces) que são comuns em várias áreas do projeto.



- `util`: Funções utilitárias como formatCurrency, formatPhone, convertTimezone, parsePhone (javascript puro).
   - `hooks`: Essa pasta é utilizada para armazenar hooks que são genéricos, têm interação com hooks do React (useState, useEffect) e normalmente reutilizáveis e qualquer projeto, exemplos: useScreenSize, useLocalStorage, useSessionStorage, useUserActive.
   - `providers`
   - `formatCurrency.js`

`validations`: são feitas as validações de formulários. Podem ser criado Schemas para a análise de regras. Pode-se utilizar a biblioteca Formic, por exemplo.


