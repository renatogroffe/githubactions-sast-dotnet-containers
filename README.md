# githubactions-sast-dotnet-containers
Exemplo de workflow do GitHub Actions com testes do tipo SAST analisando vulnerabilidades no código de uma aplicação .NET containerizida.

---

## Testes

Workflow executado com falhas:

![Workflow com falhas](img/sast-erros-01.png)

Em que foram apontados os seguintes problemas de segurança:

![Problemas de segurança](img/sast-erros-02.png)

Artefato (arquivo .pdf) gerado durante a execução da ferramenta KICS:

![Artefato do KICS](img/sast-erros-03.png)

Alertas de segurança no relatório gerado pelo KICS:

![Alertas do KICS](img/sast-erros-04.png)
