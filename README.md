qa dotnet healthchecks

Rodada completa de teste de software em um projeto C# com .NET, com foco em validação técnica, evidências reais de execução e identificação de falha em runtime.

contexto

Este repositório representa uma execução prática de QA aplicada a um sistema real.

O objetivo não foi apenas executar ferramentas, mas validar o comportamento do sistema ponta a ponta, incluindo build, testes automatizados, análise de código e funcionamento em tempo de execução.

escopo de validação
build da aplicação
execução de testes automatizados com NUnit
análise estática de código com Semgrep
enumeração de superfície web com ffuf e katana
validação funcional de endpoints via HTTP e curl
stack utilizada
C#
.NET
NUnit
ffuf
katana
httpx
curl
semgrep
GitHub Actions
estrutura do repositório
README.md
.github/workflows/ci.yml
evidencia/build
evidencia/testes_nunit
evidencia/ffuf
evidencia/katana
evidencia/httpx
evidencia/semgrep
evidencia/relatorio
evidencia/logs
evidências

As pastas em evidencia contêm os arquivos reais gerados durante a execução dos testes, incluindo:

logs de build
resultados dos testes automatizados
saída das ferramentas de análise e enumeração
registros de validação HTTP
dados de análise estática
resultado da execução
restore: ok
build: ok
testes automatizados: ok
análise estática: ok
enumeração web: ok com baixa superfície
achado principal

Foi identificada uma falha durante a validação funcional.

A aplicação não permaneceu ativa na porta 5010, impedindo a resposta dos endpoints esperados.

interpretação técnica
pipeline técnico executado com sucesso
ferramentas operando corretamente
evidências coletadas de forma consistente
falha localizada no runtime da aplicação

Este cenário caracteriza um defeito real do sistema, e não um problema no processo de teste.

conclusão

A execução demonstrou uma validação completa de QA com evidências técnicas e identificação de falha funcional.
O repositório evidencia a capacidade de testar o sistema de forma prática, indo além da execução de ferramentas e alcançando análise real de comportamento em runtime.
