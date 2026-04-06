# qa dotnet healthchecks

repositorio focado em teste de software qa sobre um projeto csharp dotnet com evidencia de execucao relatorio final e pipeline de ci

## objetivo
validar build testes automatizados analise estatica enumeracao web e comportamento funcional do sistema

## stack
csharp
dotnet
nunit
ffuf
katana
httpx
curl
semgrep
github actions

## resultado da rodada
restore ok
build ok
nunit ok
ffuf ok
katana ok com evidencia minima
semgrep ok
validacao funcional bloqueada por falha de runtime do sample na porta 5010

## achado principal
foi identificado um defeito real de execucao durante a tentativa de validacao funcional
isso caracteriza resultado legitimo de qa e nao falha do processo de teste

## estrutura do repositorio
README.md
relatorio RELATORIO_FINAL_QA.md
.github workflows ci.yml

## pipeline
o pipeline executa restore build teste e semgrep
existe uma etapa funcional opcional para o sample ate que o problema de runtime seja corrigido

## conclusao
este repositorio representa uma rodada real de qa com evidencias tecnicas e identificacao de defeito funcional
