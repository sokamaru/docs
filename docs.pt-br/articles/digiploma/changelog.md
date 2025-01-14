﻿# Histórico de versões do Digiploma

> [!NOTE]
> Este histórico por ora contém informações apenas sobre as atualizações mais recentes ao sistema. Estamos
> trabalhando para documentar as versões mais antigas.

<a name="v1-12-0" />
### 1.12.0 (2022-01-26)

* Correções de bugs
  * [AUT-143] Versão do diploma errada ao enviar webhook
  * [AUT-142] Erro de validação em regex do numero do ato

* Melhorias
  * [AUT-141] Permitir ter URLs com caminhos na URL base do modelo
  * [AUT-140] Criar novas chaves para o RVDD
  * [AUT-139] Melhorar mensagem de erro ao não preencher um campo uint como número processo da informacoesTramitacaoEmec

Atualiza modelo do banco de dados: não

<a name="v1-11-1" />
### 1.11.1 (2022-01-18)

* Correções de bugs
  * [AUT-138] Erro ao recuperar informações da documentação de registro

* Melhorias
  * [AUT-137] Novas chaves para data no RVDD e nova coluna na Pré-Visualização do aluno

Atualiza modelo do banco de dados: não

<a name="v1-11-0" />
### 1.11.0 (2021-11-30)

* Melhorias
  * [AUT-120] Adequações para versão 1.03 do XSD
  * [AUT-121] CPF do diplomado mascarado na tela de validação

Atualiza modelo do banco de dados: não

> [!WARNING]
> Breaking changes da API:
> TituloConferido: o valor "Psicólogo" não pode ser utilizado na propriedade "outroTitulo", já que foi adicionado à enum Titulo.
> DisciplinaCursada: adicionada nova propriedade obrigatória "situacao" (SituacaoDisciplina).
> "tipoAvaliacao" passa ser opcional e teve os valores "Aprovado" e "Reprovado" movidos para propriedade "situacao". Foram adicionados os valores "ConceitoRM" e "ConceitoEspecificoDoCurso".

<a name="v1-10-0" />
### 1.10.0 (2021-11-11)

* Melhorias
  * [AUT-114] Anulação definitiva de diplomas

Atualiza modelo do banco de dados: não

<a name="v1-9-2" />
### 1.9.2 (2021-11-05)

* Correções de bugs
  * [AUT-118] Chave NacionalidadeGenero faz flexão de gênero apenas se a nacionalidade informada no diploma estiver no masculino
  * [AUT-117] Mensagens de erro de RG, Outro documento de identificação, naturalidade e Situação ENADE não exibem o caminho correto
  * [AUT-116] Termo responsabilidade não deveria ser obrigatório
  * [AUT-115] Erro ao gerar diploma sem livro registro
  * [AUT-113] Correções das chaves para geração de RVDD

Atualiza modelo do banco de dados: não

<a name="v1-9-1" />
### 1.9.1 (2021-10-21)

* Correções de bugs
  * [AUT-112] Recredenciamento está como obrigatório na IES Emissora

Atualiza modelo do banco de dados: não

<a name="v1-9-0" />
### 1.9.0 (2021-10-20)

* Novas funcionalidades
  * [AUT-111] Novos condicionais e flexões de gênero

* Correções de bugs
  * [AUT-110] Erro ao enviar diploma com enums sem acento
  * [AUT-109] Erro ao gerar diploma sem Autorizacao, Reconhecimento e Renovação
  * [AUT-108] Dados do reconhecimento estão sendo exibidos como sendo da renovação de reconhecimento

Atualiza modelo do banco de dados: não

<a name="v1-8-0" />
### 1.8.0 (2021-10-13)

* Novas funcionalidades
  * [AUT-106] Adicionar upload de novo arquivo no modelo para impressão em papel timbrado

Atualiza modelo do banco de dados: sim

<a name="v1-7-0" />
### 1.7.0 (2021-10-01)

* Novas funcionalidades
  * [AUT-103] Adicionar filtro por status e data na listagem de diplomas

* Melhorias
  * [AUT-104] Adicionar nova chave para fazer flexão de gênero do titulo conferido ao estudante
  * [AUT-100] Aceitar flow id na API de criação de diplomas

* Correções de bugs
  * [AUT-105] Tela de validação apresenta erros caso o diploma não esteja válido

Atualiza modelo do banco de dados: não

<a name="v1-6-0" />
### 1.6.0 (2021-09-17)

* Novas funcionalidades
  * [AUT-95] Download em lote dos documentos de Diploma
  * [AUT-26] Captcha de proteção para consulta pública

* Melhorias
  * [AUT-93] Assinatura de diploma com requisitos de certificados

Atualiza modelo do banco de dados: não
