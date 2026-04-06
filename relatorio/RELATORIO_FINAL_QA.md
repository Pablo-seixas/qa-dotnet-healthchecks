# relatorio final de qa

## projeto
AspNetCore.Diagnostics.HealthChecks

## objetivo
executar validacao de qa em projeto csharp com foco em build testes analise estatica e validacao funcional

## ambiente
arch linux
dotnet sdk
node npm

## ferramentas utilizadas
nunit
ffuf
katana
httpx
curl
semgrep

## atividades executadas
criacao da estrutura de evidencias
registro do ambiente
correcao de caminho do repositorio para evitar erro com caractere especial
restore com solution correta
build com solution correta
criacao e execucao de testes nunit
execucao de ffuf
execucao de katana
execucao de semgrep
tentativa de validacao funcional com httpx e curl

## resultado por etapa
restore ok
build ok
nunit ok
ffuf ok
katana ok com evidencia minima
semgrep ok
http funcional bloqueado

## problema encontrado
aplicacao sample nao permaneceu ouvindo na porta 5010 durante a validacao funcional
curl retornou falha de conexao
isso indica falha de runtime da aplicacao durante o teste funcional

## leitura tecnica
camada de build aprovada
camada de testes automatizados aprovada
camada de analise estatica aprovada
camada de superficie web aprovada com ressalva
camada funcional reprovada por indisponibilidade da aplicacao sample

## conclusao final
qa tecnico aprovado com achado funcional critico
houve evidencias suficientes para demonstrar que o sistema compila e os testes automatizados executam
houve evidencias suficientes para demonstrar defeito real no runtime do sample durante a validacao funcional

## proximo passo recomendado
corrigir a execucao do sample
reexecutar validacao funcional de health healthz e metrics
promover validacao funcional para etapa obrigatoria do pipeline
