---
id: how-to-contribute
title: Como contribuir
layout: contributing
permalink: docs/how-to-contribute.html
next: codebase-overview.html
redirect_from:
  - "contributing/how-to-contribute.html"
  - "tips/introduction.html"
---

React � um dos primeiros projetos de c�digo aberto do Facebook que est� sendo desenvolvido muito ativamente, al�m de ser usado para entregar c�digo para todos em [facebook.com](https://www.facebook.com). N�s ainda estamos trabalhando para tornar esse projeto mais transparente e f�cil poss�vel, mas ainda n�o est�mos l�. Esperamos que essa documenta��o torne esse processo de contribui��o mais clara e responda algumas perguntas que voc� possa ter.

### [C�digo de Conduta](https://code.facebook.com/codeofconduct) {#code-of-conduct}

O Facebook adotou um c�digo de contuda que esperamos que todos os participantes desse projeto adotem. Por favor, [leia o texto completo](https://code.facebook.com/codeofconduct) para que voc� possa entender quais a��es ser�o ou n�o toleradas.

### Desenvolvimento Aberto {#open-development}

Todo trabalho no React acontece diretamente no [GitHub](https://github.com/facebook/react). Tanto membros do ***Core Team*** quanto contribuidores externos devem enviar ***pull requests*** que v�o passar pelo mesmo processo de revis�o.

### Organiza��o de ***branches*** {#branch-organization}

N�s buscaremos fazer o nosso melhor para manter [branch `master`](https://github.com/facebook/react/tree/master) organizada, com testes passando todas as vezes. Mas para garantir que seremos r�pidos, n�s faremos mudan�as na API nas quais suas aplica��es podem n�o ser compat�veis. N�s recomendamos que voc� use [a vers�o est�vel do React](/downloads.html).

Se voc� enviar uma ***pull request***, por favor fa�a contra a branch `master`. N�s mantemos ***branches*** est�veis para vers�es maiores separadamente, mas n�o aceitamos ***pull requests*** para elas diretamente. Ao inv�s disso, n�s fazemos ***cherry-pick*** de mudan�as que n�o quebrem o c�digo da `master` para a �ltima vers�o mais est�vel.

### Versionamento Sem�ntico {#semantic-versioning}

O Reat segue o [versionamento sem�ntico](http://semver.org/). Buscar lan�ar vers�es de ***patch*** para corre��es de bugs, vers�es secund�rias (minor version) para novos recursos e vers�es principais (major version) para qualquer altera��o de quebra. Quando fazemos altera��es significativas, tamb�m introduzimos alguns avisos de descontinuidade em uma vers�o secund�ria para que nossos usu�rios tenham conhecimento sobre as pr�ximas altera��es e migrem seu c�digo com anteced�ncia.

N�s marcamos com ***tags*** qualquer ***pull request*** com um marcador que indica se a altera��o deve ir para o pr�ximo [patch](https://github.com/facebook/react/pulls?q=is:open+is:pr+label:semver-patch), [vers�o secund�ria (minor version)](https://github.com/facebook/react/pulls?q=is:open+is:pr+label:semver-minor) ou em uma [vers�o principal (major version)](https://github.com/facebook/react/pulls?q=is:open+is:pr+label:semver-major). N�s lan�amos novas vers�es de ***patch*** a cada poucas semanas, vers�es secund�rios a cada poucos meses e vers�es principais uma ou duas vezes por ano.

Toda mudan�a significativa � documentada na [***changelog***](https://github.com/facebook/react/blob/master/CHANGELOG.md).

### Bugs {#bugs}

#### Onde encontrar problemas conhecidos {#where-to-find-known-issues}

N�s estamos utilizando as [GitHub Issues](https://github.com/facebook/react/issues) para nossas p�ginas p�blicas. N�s vamos ficar de olho e tentar manter claro quando estamos trabalhando internamente na corre��o de algum bug. Antes de preencher uma nova tarefa, verifique se o problema j� existe.

#### Relatando novos problemas {#reporting-new-issues}

A melhor maneira de corrigir o problema � fornecer um caso de teste reduzido. Este [template no JSFiddle](https://jsfiddle.net/Luktwrdm/) � um excelente ponto de partida.

#### Bugs de seguran�a {#security-bugs}

O Facebook tem um [programa de recompensas](https://www.facebook.com/whitehat/) para a divulga��o segura de bugs de seguran�a. Com isso em mente, n�o reporte esses problemas de forma p�blica; Percorra o processo descrito nessa p�gina.

### Como entrar em contato {#how-to-get-in-touch}

* IRC: [#reactjs on freenode](https://webchat.freenode.net/?channels=reactjs)
* F�rum de Discuss�o: [discuss.reactjs.org](https://discuss.reactjs.org/)

H� tamb�m uma comunidade ativa de usu�rios do React na plataforma no [Discord](http://www.reactiflux.com/) caso voc� precise de ajuda.

### Propondo uma altera��o {#proposing-a-change}

Se voc� pretende alterar a API p�blica ou fazer altera��es n�o triviais na implementa��o, recomendamos [abrir uma ***issue***](https://github.com/facebook/react/issues/new). Isso nos permite chegar a um acordo sobre sua proposta antes de colocar um esfor�o significativo nela.

Se voc� est� apenas corrigindo um bug, n�o tem problema em enviar uma ***pull request*** diretamente, mas ainda sim recomendamos abrir uma ***issue*** com detalhes sobre o que voc� est� corrigindo. Isso � �til caso n�o aceitemos essa corre��o espec�fica, mas queremos acompanhar o problema.

### Sua primeira ***Pull Request*** {#your-first-pull-request}

Trabalhando em sua primera ***Pull Request***. Voc� pode aprender como desta s�rie de v�deos gratuitos:

**[Como contribuir para um projeto de c�digo aberto no GitHub](https://egghead.io/series/how-to-contribute-to-an-open-source-project-on-github)**

Para ajudar voc� a se familiarizar com o nosso processo de contribui��o, temos uma lista de [boas primeiras ***issues***](https://github.com/facebook/react/issues?q=is:open+is:issue+label:"good+first+issue") que cont�m erros que t�m um escopo relativamente limitado. Este � um �timo lugar para come�ar.

Se voc� decidir corrigir um bug, por favor, verifique o t�pico do coment�rio caso algu�m j� esteja trabalhando em uma corre��o. Se ningu�m estiver trabalhando no momento, por favor deixe um coment�rio dizendo que voc� pretende trabalhar nele para que outras pessoas n�o dupliquem sem querer seu esfor�o.

Se algu�m assumir uma ***issue***, mas n�o fizer o acompanhamento por mais de duas semanas, n�o h� problema em voc� assumir, mas mesmo assim voc� ainda deve deixar um coment�rio.

### Enviando uma ***Pull Request*** {#sending-a-pull-request}


O Core Team est� monitorando as ***pull requests***. Analisaremos seu envio e fazermos o ***merge***, solicitaremos altera��es ou podemos fech�-la com uma explica��o plaus�vel. Para altera��es de API, podemos precisar corrigir nossos usos internos no Facebook.com, o que pode causar algum atraso. Faremos o nosso melhor para fornecer atualiza��es e feedback durante todo o processo.

**Antes de enviar a sua pull request,** certifique-se de ter feito os seguintes passos:

1. Fala fork do [reposit�rio oficial](https://github.com/facebook/react) and criou sua branch da `master`.
2. Execute `yarn` no reposit�rio ra�z.
3. Se voc� corrigiu um bug ou um c�digo adicionado que deve ser testado, adicione testes!
4. Certifique-se de que a su�te de teste passe (`yarn test`). Dica: `yarn test --watch TestName` � �til no desenvolvimento.
5. Execute `yarn test-prod` para testar no ambiente de produ��o. Suporta as mesmas op��es que `yarn test`.
6. Se voc� precisar de um depurador, execute `yarn debug-test --watch TestName`, abra `chrome://inspect`e aperte em "Inspecionar".
7. Formate seu c�digo com [prettier](https://github.com/prettier/prettier) (`yarn prettier`).
8. Certifique-se de que seus c�digos foram verificados com linters (`yarn lint`). Dica: `yarn linc` verifica somente os arquivos alterados.
9. Rode o [Flow](https://flowtype.org/) para typechecks (`yarn flow`).
10. Se ainda n�o fez, preencha o CLA.

### Licen�a de Acordo de Contribuidor (***Contributor License Agreement*** - CLA) {#contributor-license-agreement-cla}

Para aceitar sua ***pull request***, precisamos que voc� envie um CLA. Voc� s� precisa fazer isso uma vez, ent�o se voc� fez isso para outro projeto de c�digo aberto do Facebook, voc� est� pronto para continuar. Se voc� estiver enviando uma ***pull request*** pela primeira vez, nos informe que voc� concluiu o CLA e ent�o podemos fazer uma verifica��o cruzada com seu GitHub

**[Preencha sua CLA aqui.](https://code.facebook.com/cla)**

### Pr�-requisitos de contribui��o {#contribution-prerequisites}

* Possuir o [Node](https://nodejs.org) instalado na vers�o v8.0.0+ e [Yarn](https://yarnpkg.com/en/) na vers�o v1.2.0+.
* Voc� deve ter o `gcc` instalado ou est� confort�vel em instalar um compilador, se necess�rio. Algumas de nossas depend�ncias podem exigir uma etapa de compila��o. No OS X, as Ferramentas de Linha de Comando do Xcode cobrir�o isso. No Ubuntu, `apt-get install build-essential` instalar� os pacotes requeridos. Comandos semelhantes devem funcionar em outras distribui��es Linux. O Windows ir� requerer alguns passos adicionais, veja as instru��es de instala��o do [node-gyp](https://github.com/nodejs/node-gyp#installation) para detalhes.
* Voc� deve ser familiarizado com o Git.

### Fluxo de Trabalho de Desenvolvimento {#development-workflow}

Depois de clonar o React, execute `yarn` para buscar suas depend�ncias.E nt�o, voc� pode executar v�rios comandos:

* `yarn lint` verifica o estilo de c�digo.
* `yarn linc` funciona como o `yarn lint` mas �w mais r�pido porque verifica apenas os arquivos que diferem na sua ***branch***.
* `yarn test` executa o conjunto de testes completo.
* `yarn test --watch` executa um observador de testes interativo.
* `yarn test <pattern>` executa testes com nomes de arquivos correspondentes.
* `yarn test-prod` executa testes no ambiente de produ��o. Suporta todas as mesmas op��es que o `yarn test`.
* `yarn debug-test` � como `yarn test` mas com um depurador. Abra `chrome://inspect` e clique em "Inspecionar".
* `yarn flow` executa o typecheck do [Flow](https://flowtype.org/) .
* `yarn build` cria uma pasta `build` com todos os pacotes.
* `yarn build react/index,react-dom/index --type=UMD` cria compila��es UMD somente com o React e ReactDOM.

Recomendamos executar o `yarn test` (ou suas varia��es acima) para garantir que voc� n�o introduza nenhuma regress�o enquanto trabalha na sua mudan�a. No entanto, pode ser �til testar sua vers�o do React em um projeto real.

Primeiro, execute `yarn build`. Isto ir� produzir pacotes pr�-constru�dos na pasta `build`, bem como ir� preparar pacotes npm dentro da pasta `build/packages`.

A maneira mais f�cil de testar suas altera��es � rodar `yarn build react/index,react-dom/index --type=UMD` e depois abrir `fixtures/packaging/babel-standalone/dev.html`. Este arquivo j� usa o `react.development.js` a partir da pasta `build` para que ele possa pegar suas altera��es.

Se voc� quiser testar suas altera��es em seu projeto React j� existente, voc� pode copiar `build/dist/react.development.js`, `build/dist/react-dom.development.js` ou qualquer outro build em seu aplicativo e us�-los em vez da vers�o est�vel. Se o seu projeto usa o React do npm, voc� pode excluir `react` e` react-dom` em suas depend�ncias e usar `yarn link` para apont�-los para sua pasta` build` local:

```sh
cd ~/path_to_your_react_clone/build/node_modules/react
yarn link
cd ~/path_to_your_react_clone/build/node_modules/react-dom
yarn link
cd /path/to/your/project
yarn link react react-dom
```

Toda vez que voc� executar `yarn build` na pasta React, as vers�es atualizadas aparecer�o no` node_modules` do seu projeto. Voc� pode ent�o reconstruir seu projeto para testar suas altera��es.

Ainda exigimos que sua ***pull request*** contenha testes de unidade para qualquer nova funcionalidade. Dessa forma, podemos garantir que n�o quebremos seu c�digo no futuro.

### Guia de estilo {#style-guide}

Usamos um formatador de c�digo autom�tico chamado [Prettier](https://prettier.io/). Execute o `yarn prettier` depois de fazer qualquer altera��o no seu c�digo.

Ent�o, nosso linter ir� capturar a maioria dos problemas que possam existir em seu c�digo. Voc� pode verificar o status do seu estilo de c�digo simplesmente executando `yarn linc`.

No entanto, ainda existem alguns estilos que o linter n�o consegue captar. Se voc� n�o tem certeza sobre alguma coisa, veja o [Guia de Estilos do Airbnb](https://github.com/airbnb/javascript) para te direcionar no caminho certo.

### V�deo introdut�rio {#introductory-video}

Voc� pode estar interessado em assistir [este pequeno v�deo](https://www.youtube.com/watch?v=wUpPsEcGsg8) (26 minutos), que apresenta uma introdu��o sobre como contribuir para o React.

#### Destaques no v�deo: {#video-highlights}
- [4:12](https://youtu.be/wUpPsEcGsg8?t=4m12s) - Construindo e testando Reagir localmente
- [6:07](https://youtu.be/wUpPsEcGsg8?t=6m7s) - Criando e enviando ***pull requests***
- [8:25](https://youtu.be/wUpPsEcGsg8?t=8m25s) - Organizando c�digo
- [14:43](https://youtu.be/wUpPsEcGsg8?t=14m43s) - React npm registry
- [19:15](https://youtu.be/wUpPsEcGsg8?t=19m15s) - Adicionando novos recursos do React

Para obter uma vis�o geral realista do que � o sentimento de contribuir para o React pela primeira vez, confira [essa palestra interessante no ReactNYC](https://www.youtube.com/watch?v=GWCcZ6fnpn4).

### Pedido de Coment�rios (Request for Comments - RFC) {#request-for-comments-rfc}

Muitas altera��es, incluindo corre��es de bugs e melhorias na documenta��o, podem ser implementadas e revisadas por meio do fluxo de trabalho normal de ***pull requests*** do GitHub.

Algumas mudan�as, entretanto, s�o "substanciais", e pedimos que estas sejam submetidas a um pequeno processo de design e produzam um consenso entre o Core Team do React.

O processo "RFC" (pedido de coment�rios) destina-se a fornecer um caminho consistente e controlado para que novos recursos entrem no projeto. Voc� pode contribuir visitando o reposit�rio [rfcs](https://github.com/reactjs/rfcs).

### Licen�a {#license}

Ao contribuir com o React, voc� concorda que suas contribui��es ser�o licenciadas sob sua licen�a do MIT.

### O que vem a seguir? {#what-next}

Leia a [pr�xima se��o](/docs/codebase-overview.html) para saber como a base de c�digo � organizada.
