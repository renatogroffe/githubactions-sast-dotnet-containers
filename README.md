# githubactions-sast-dotnet-containers
Exemplo de workflow do GitHub Actions com testes do tipo SAST analisando vulnerabilidades no código de uma aplicação .NET containerizida.

---

## Testes

Workflow executado com falhas:

![Workflow com falhas](img/sast-erros-01.png)

Em que foram apontados os seguintes problemas de segurança:

![Problemas de segurança](img/sast-erros-02.png)

Artefato (arquivo .pdf) gerado durante a execução da ferramenta [**KICS**](https://kics.io/index.html):

![Artefato do KICS](img/sast-erros-03.png)

Alertas de segurança no relatório gerado pelo KICS:

![Alertas do KICS](img/sast-erros-04.png)

Os problemas a serem corrigidos foram marcados como TO-DOs:

![Problemas a serem corrigidos](img/to-dos-01.png)

Para facilitar isto fez uso das extensões [**Todo Tree**](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree) e [**TODO Highlight**](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)

![Extensões do Visual Studio Code indicadas](img/vscode-01.png)

Workflow executado com sucesso após correções:

![Workflow executado após correções](img/correcoes-01.png)

Testes executados com sucesso utilizando um cluster emulado via [**kind**](https://kind.sigs.k8s.io/):

![Testes via kind](img/correcoes-02.png)

Alertas de segurança solucionados:

![Alertas solucionados](img/correcoes-03.png)
