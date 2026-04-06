# qa dotnet healthchecks

repositorio focado em teste de software qa com evidencias reais geradas em execucao local

## objetivo
validar build testes automatizados analise estatica enumeracao web e validacao funcional

## estrutura
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

## resultado final da rodada
restore ok
build ok
nunit ok
ffuf ok
katana ok com evidencia minima
semgrep ok
validacao funcional bloqueada por falha de runtime do sample na porta 5010

## observacao
as pastas em evidencia contem os arquivos reais produzidos durante a execucao dos comandos no ambiente local
