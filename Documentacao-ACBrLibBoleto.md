ACBrLibBoleto (ACBrLibBoleto.html)/

# Configurações da Biblioteca

## Configurações da Biblioteca

Neste tópico você vai encontrar todas as chaves possíveis da biblioteca e também uma explicação para
cada chave, algumas configurações você vai encontrar no tópico: Configurações da Biblioteca (Geral) (Geral.html) e
Configurações DFe (DFe.html). Para BoletoWeb é necessário realizar as Configurações SSLHttpLib em [DFe].

**Obs.:** **_Para Integração Bancária por WebService ou API, consulte o tópico abaixo para saber os
bancos com essa disponibilidade e as configurações específicas para integração WEB._**
https://www.projetoacbr.com.br/forum/topic/57991-acbrboleto-via-webservice/
(https://www.projetoacbr.com.br/forum/topic/57991-acbrboleto-via-webservice/)

```
[BoletoBancoConfig]
```
```
CHAVE DESCRIÇÃO
```

**TipoCobranca**

```
Define qual o Banco será utilizado seguindo os códigos abaixo (É necessário a
definição do Banco antes de utilizar qualquer método do componente Boleto):
0 - Nenhum
1 - Banco
do Brasil
2 -
Santander
3 - Caixa
Econômica
Federal
(Convênio
SIGCB)
4 - Caixa
Econômica
Federal
(Convênio
SICOB)
5 -
Bradesco
6 - Itaú
7 - Banco
Mercantil
8 - Sicred
9 - Bancoob
10 -
Banrisul
11 -
Banestes
12 - HSBC
13 - Banco
do Nordeste
14 - Banco
BRB
15 -
BicBanco
```
```
16 - BradescoSICOOB
17 - BancoSafra
18 - SafraBradesco
19 - BancoCECRED
20 - BancoDaAmazonia
21 -
BancoDoBrasilSICOOB
22 - Uniprime
23 - UnicredRS
24 - Banese
25 - CrediSIS
26 - UnicredES
27 - BancoCresolSCRS
28 - CitiBank
29 - BancoABCBrasil
30 - Daycoval
31 - UniprimeNortePR
```
```
32 - BancoPine
33 -
BancoPineBradesco
34 - UnicredSC
35 - BancoAlfa,
36 - BancoDoBrasilAPI
37 - BancoDoBrasilWS
38 - BancoCresol
39 - MoneyPlus
40 - BancoC
41 - BancoRendimento
42 - BancoInter
43 -
BancoSofisaSantander
44 - BS
45 - PenseBankAPI
46 - BTGPactual
47 - BancoOriginal
```
```
48 - BancoVotorantin
49 - BancoPefisa
50 - BancoFibra
51 - BancoSofisaItau
52 -
BancoIndustrialBrasil
53 -
BancoAthenaBradesco
54 - BancoQITechSCD
55- BancoUY
56- BancoBocomBBM
57- BancoSicoob,
58- BancoSisprime,
59- BancoAilos
```
**Numero**

```
O Código utilizado pelo Banco (Caso não informado será preenchido
automaticamente pelo componente, baseado nas configurações da classe do banco
selecionado em "TipoCobrança".
```
**NumeroCorrespondente** O Código do Correspondente Bancário utilizado pelo Banco. (Utilizado apenas por
algumas Cooperativas de Crédito).

**LayoutVersaoArquivo** O Número da Versão do Layout do arquivo de Remessa (Não preencher se não
necessário).

**LayoutVersaoLote** O Número da Versão do Lote do arquivo de Remessa (Não preencher se não
necessário).

**LocalPagamento** Define o local de pagamento a ser impresso no boleto desse banco.

**OrientacaoBanco** Define uma String com as orientações do Banco para ser impresso no Boleto.

**Digito** O Dígito do Banco (Não preencher se não existir).


**CasasDecimaisMoraJuros** A Quantidade de casa decimais do campo juros/mora.

**CIP** Código usado por alguns bancos para impressão no boleto.

```
[BoletoCedenteConfig]
```
```
CHAVE DESCRIÇÃO
```
**Agencia** Define o Numero da Agência do Cedente.

**AgenciaDigito** Define o Numero do Dígito da Agência.

**Conta** Define o Numero da Conta do Cedente.

**ContaDigito** Define o Numero do Digito da Agência.

**DigitoVerificadorAgenciaConta** Define o Digito verificador da Agência e Conta (Utilizado apenas por alguns
Bancos).

**Convenio** Define o Número do Convénio (deve ser verificado com o Banco).

**CodigoCedente** Define o Código do Cedente (deve ser verificado com o Banco).

**CodigoTransmissao** Define o Código de Transmissão (deve ser verificado com o Banco, quando
existir).

**Modalidade** Define o Código da Modalidade (deve ser verificado com o Banco, quando
existir).

**ResponEmissao**

```
Define o Responsável pela emissão do boleto, conforme Códigos abaixo:
0 - Cliente Emite
1 - Banco Emite
2 - Banco Reemite
3 - Banco não Reemite
```
**TipoCarteira**

```
Define o Responsável pela emissão do boleto, conforme Códigos abaixo:
0 - Carteira Simples
1 - Carteira Registrada
2 - Carteira Eletrônica
```
**TipoDocumento**

```
Define o Tipo de Documento, conforme Códigos abaixo:
0 - Documento Tradicional
1 - Documento Escritural
```
**TipoInscricao**

```
Define o Tipo de Inscrição, conforme Códigos abaixo:
0 - Pessoa Física
1 - Pessoa Jurídica
2 - Outros
```
**CaracTitulo**

```
Define Características de Cobrança do Título, conforme Códigos abaixo:
0 - Cobrança Simples
1 - Cobrança Vinculada
2 - Cobrança Caucionada
3 - Cobrança Descontada
4 - Cobrança Vendor
5 - Cobrança Simples (Rápida com Registo)
6 - Cobrança Caucionada (Rápida com Registro)
```

**CodigoNegativacao**

```
Define o Código de Negativação, conforme Códigos abaixo:
0 - Nenhum
1 - Protestar Corrido
2 - Protestar Uteis
3 - Não Protestar
4 - Negativar
5 - Não Negativar
6 - Cancelamento
```
**CNPJCPF** O Número do CNPJ ou CPF do Cedente.

**Nome** O Nome do Cedente.

**Logradouro** O Endereço do Cedente.

**NumeroRes** O Número Residencial do Cedente.

**Complemento** O Complemento de Endereço do Cedente.

**Bairro** O Bairro do Cedente.

**Cidade** A Cidade do Cedente.

**CEP** O CEP do Cedente.

**UF** A UF do Cedente.

**Telefone** O telefone do Cedente.

**IdentDistribuicao**

```
Utilizado por alguns bancos para definir quem distribui o boleto:
0 - tbBancoDistribui
1 - tbClienteDistribui
```
**Operacao** Utilizado por alguns bancos para definir dados adicionais.

**ChavePIX** Informe chave pix.

**TipoChavePIX**

```
Define o tipo de chave pix abaixo:
0 - Nenhum
1 - Email
2 - CPF
3 - CNPJ
4 - Celular
5 - Aleatória
```
```
[BoletoDiretorioConfig]
```
```
CHAVE DESCRIÇÃO
```
**LayoutRemessa**

```
Define o Modelo do CNAB para geração da Remessa, conforme códigos
abaixo:
```
```
0 - CNAB
1 - CNAB
```
**DirArqRemessa** Define o Diretório para geração do arquivo de remessa.

**DirArqRetorno** Define o Diretório para leitura do arquivo de retorno.


**NomeArqRemessa** Define o Nome do Arquivo de Remessa a ser gerado pelo componente
Boleto.

**NomeArqRetorno** Define o Nome do Arquivo de Retorno a ser lido pelo componente Boleto.

**NumeroArquivo** Define o numero sequencial do Arquivo Remessa a ser gerado. (Também
pode ser parametrizado via comando).

**DataArquivo** Data de geração do Arquivo de Remessa. (Não preencher se não utilizado).

**DataCreditoLanc** Data de Créditos de Lançamento do Arquivo de Retorno. (Não preencher se
não utilizado).

**ImprimirMensagemPadrao**

```
Define a Impressão ou não de Mensagens Padrão no Boleto:
0 - Não
1 - Sim
```
**LeCedenteRetorno** Define se Lê os dados do Cedente para validar o Arquivo de Retorno.

**RemoveAcentosArqRemessa**

```
Define se deve ou não remover os acentos no arquivo de remessa:
0 - Não
1 - Sim
```
**PrefixArqRemessa** Define um prefixo para o nome do arquivo de remessa (exclusivo Banco
Daycoval).

```
[BoletoBancoFCFortesConfig]
```
```
CHAVE DESCRIÇÃO
```
**NomeArquivo** Define o Nome do Arquivo para geração do Boleto em PDF (Informar o
Path Completo ex: c:\temp\BoletoPDF.pdf).

**DirLogo** Define o Diretório onde está localizado os Logotipos dos Bancos.

**Filtro**

```
Define o Filtro para geração do Boleto conforme Código abaixo:
0 - Nenhum
1 - PDF
2 - HTML
3 - JPG
```
**Layout**

```
Define o tipo de Layout para Impressão do Boleto conforme Código
abaixo:
0 - Padrão
1 - Carnê
2 - Fatura
3 - Padrão Entrega
4 - Recibo Topo
5 - Padrão Entrega
6 - FaturaDetalhe
7 - Termica80mm
8 - PadraoPIX
9 - PrestaServicos
```

**MostrarPreview**

```
Define a opção para Mostrar ou não o Preview:
0 - Não
1 - Sim
```
**MostrarProgresso**

```
Define a opção para Mostrar Progresso de Impressão:
0 - Não
1 - Sim
```
**MostrarSetup**

```
Define a opção para Mostrar Setup de Impressão:
0 - Não
1 - Sim
```
**NumeroCopias** Define o Número de Cópias para Impressão.

**PrinterName** Nome da impressora para impressão.

**SoftwareHouse** Nome da SoftwareHouse.

**AlterarEscalaPadrao**

```
Permite alterar a escala padrão para geração da impressão
0 - Não
1 - Sim
```
**NovaEscala** Valor da nova escala padrão (default = 96)

**CalcularNomeArquivoPDFIndividual**

```
Define se o nome do PDF gerado individualmente deve ser calculado
utilizando o número do documento, caso contrário usa o nome informado
nos parâmetros.
0 - Não
1 - Sim
```
**MargemInferior** Define a margem inferior da impressão.

**MargemSuperior** Define a margem superior da impressão.

**MargemEsquerda** Define a margem esquerda da impressão.

**MargemDireita** Define a margem direita da impressão.

```
[BoletoCedenteWS]
```
```
CHAVE DESCRIÇÃO
```
**ClientID** CredencialD fornecida pelo Banco para integração WebService.

**ClientSecret** Chave Credencial fornecida pelo Banco para integração WebService.

**KeyUser** Gerada pelo Banco para o cadastro do Cliente.

**Scope** Scope do Serviço da API ou WebService de Cada Banco.

**IndicadorPix**

```
Indica se Realiza intergação do Boleto por Pix (Apenas API Banco do Brasil):
0 - Não
1 - Sim
```
```
[BoletoWebSevice]
```

### CHAVE DESCRIÇÃO

**PathGravarRegistro** Define se será gerado o log de cada requisição:

**Ambiente**

```
Ambiente
0 - Produção
1 - Homologaçao
```
**Operação**

```
Tipo de Operação:
0 - Inclusão
1 - Alteração
2 - Baixa
3 - Consulta
4 - ConsultaDetalhada
5 - PIXCriar
6 - PIXCancelar
7 - PIXConsultar
8 - Cancelar
9 - Ticket
```
**VersaoDF** Versão do layout Serviço Web (Não informar se não existir).

**UseCertificateHTTP**

```
Define se utiliza ou não certificado Digital para integração com o Banco (Default
todos são 0):
0 - Não
1 - Sim
```
**SSLType**

```
Define o tipo de comunicação segura a ser utilizada:
0 = LT_all
1 = LT_SSLv
2 = LT_SSLv
3 = LT_TLSv
4 = LT_TLSv1_
5 = LT_TLSv1_
6 = LT_SSHv
```
**Timeout** Define o tempo em milissegundos de espera por uma resposta do webservice:
Padrão = 5000

**ArquivoCRT** Caminho do Arquivo CRT (Informar o Path Completo ex: c:\temp\ArquivoCRT.crt).

**ArquivoKEY** Caminho do Arquivo KEY (Informar o Path Completo ex:c:\temp\ArquivoKEY.key).

**LogNivel**

```
Define o tipo de log utilizado para monitorar as Requisições Web:
0 - logNenhum
1 - logSimples
2 - logNormal
3 - logCompleto
4 - logParanoico
```
**PathGravarRegistro**

```
Define o caminho onde ver ser salvo o arquivo de log das Requisições WEB,
exemplo:
c:\temp\
```

```
NomeArquivoLog Define o nome do arquivo log de sua preferência, exemplo:
MeuArquivoLog.TXT
```
```
Created with the Personal Edition of HelpNDoc: Full-featured multi-format Help generator
(https://www.helpndoc.com/help-authoring-tool)
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>


```
ACBrLibBoleto (ACBrLibBoleto.html)/Informações (Informacoes1.html)/
```
# Como Emitir um Boleto

## Passos para imprimir Boletos

```
A impressão dos boletos pode ser feita em diversas sequências diferentes, utilizando-se os comandos separados
para cada passo ou as funções extras do comando IncluirTitulo.
Para que ao imprimir novos títulos os antigos não sejam impressos novamente, sempre utilize o comando
LimparLista.
```
```
Modo 1 - Fazendo os passos separadamente
```
```
1 - Limpe a lista de títulos.
Exemplo: BOLETO_LimparLista();
```
```
2 - Utilize o comando ConfiguraDados para configurar as informações da Conta e do Cedente, pode ser informando
o Path do arquivo INI ou então o seu conteúdo.
Exemplo: BOLETO_ConfigurarDados("c:\cedente.ini (ModeloCedenteINI.html)" );
```
```
3 - Utilize o comando IncluirTitulo para adicionar os boletos a serem impressos, pode ser informando o Path do
arquivo INI ou então o seu conteúdo.
Exemplo: BOLETO_ IncluirTitulos ("c:\titulos.ini (ModeloTituloINI.html)") ;
```
```
4 - Utilize o comando Imprimir para que os boletos enviados no comando IncluirTitulo sejam impressos.
Exemplo: BOLETO_Imprimir();
```
```
Modo 2 - Informando os dados da Conta e Cedente através do IncluirTitulo
```
```
1 - Limpe a lista de títulos.
Exemplo: BOLETO_LimparLista();
```
```
2 - Utilize o comando IncluirTitulo, informando o caminho para o arquivo com os títulos, para informar os Dados do
Conta e do Cedente e também para adicionar os boletos a serem impressos.
Exemplo: BOLETO_ IncluirTitulos ("c:\cedente_titulos.ini (ModeloCedente_TitulosINI.html)");
```
```
3 - Utilize o comando Imprimir para que os boletos enviados no comando IncluirTitulo sejam impressos.
Exemplo: BOLETO_Imprimir();
```
```
Modo 3 - Utilizando apenas o IncluirTitulo
```
```
1 - Limpe a lista de títulos.
Exemplo: BOLETO_LimparLista();
```
```
2 - Neste modo, todas as operações necessárias são feitas através do comando IncluirTitulo, para tanto, utilize o
comando da seguinte maneira.
Exemplo: BOLETO_ IncluirTitulos ("c:\cedente_titulos.ini (ModeloCedente_TitulosINI.html)", "I");
```
27/10/24, 15:44 Como Emitir um Boleto

https://acbr.sourceforge.io/ACBrLib/ComoEmitirumBoleto.html 1 / 2


```
O arquivo titulos.ini, deverá conter as informações referentes a Conta e ao Cedente e também os boletos a serem
impressos.
O parâmetro "I" significa que após efetuar a configuração e incluir os títulos, em seguida deve ser feita a impressão
dos mesmos.
```
```
Created with the Personal Edition of HelpNDoc: Single source CHM, PDF, DOC and HTML Help creation
(https://www.helpndoc.com/help-authoring-tool)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:44 Como Emitir um Boleto

https://acbr.sourceforge.io/ACBrLib/ComoEmitirumBoleto.html 2 / 2

```
ACBrLibBoleto (ACBrLibBoleto.html)/Informações (Informacoes1.html)/
```
# Modelo Cedente.INI

```
[Cedente]
Nome=SAO JOAO LTDA.
CNPJCPF= 99.999.999/9999-
Logradouro=Rua Evaristo Mendes
Numero=
Bairro=Centro
Cidade=Tatui
CEP=18.270-
Complemento=Sala 10
UF=SP
RespEmis=
TipoPessoa=
CodigoCedente=
LayoutBol=
CaracTitulo=
TipoCarteira=
TipoDocumento=
Modalidade=
CodTransmissao=
Convenio=
PIX.TipoChavePix=
PIX.Chave=teste@testechave.com
```
```
[Conta]
Conta=
DigitoConta=
Agencia=
DigitoAgencia=
DigitoVerificadorAgenciaConta=
```
```
[Banco]
Numero=
CNAB=
TipoCobranca=
NumeroCorrespondente=
VersaoArquivo=
VersaoLote=
```
```
[WEBSERVICE]
ClientID=
ClientSecret=
KeyUser=
Scope=
IndicadorPix=
Ambiente=
SSLHttpLib=
ArquivoKEY=
```
27/10/24, 15:45 Modelo Cedente.INI

https://acbr.sourceforge.io/ACBrLib/ModeloCedenteINI.html 1 / 2


```
ArquivoCRT=
```
```
Created with the Personal Edition of HelpNDoc: Easy EBook and documentation generator
(https://www.helpndoc.com)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:45 Modelo Cedente.INI

https://acbr.sourceforge.io/ACBrLib/ModeloCedenteINI.html 2 / 2

```
ACBrLibBoleto (ACBrLibBoleto.html)/Informações (Informacoes1.html)/
```
# Modelo Titulo.INI

```
[Titulo1]
NumeroDocumento =
NossoNumero =
NossoNumeroCorrespondente=4cac8ea0-a960-4ac4-af55-c6b05728f3x0 ;; Obrigatório - API PIX do BANCO
INTER para realizar APENAS CONSULTAS, ALTERACOES E BAIXAS (ESTE VALOR É INFORMADO NO
RETORNO DA INCLUSAO)
Carteira =
ValorDocumento =100,
Vencimento =10/09/
DataDocumento=10/08/
DataProcessamento=10/08/
DataAbatimento=05/09/
DataDesconto=07/09/
DataMoraJuros=12/09/
DiasDeProtesto=
DiasDeNegativacao=
DataProtesto=10/10/
DataNegativacao=10/10/
DataMulta=10/10/
DataBaixa=10/10/
ValorAbatimento=5,
ValorDesconto=0,
ValorMoraJuros=0,
ValorIOF=3,
ValorOutrasDespesas=2,
MultaValorFixo=
PercentualMulta=05,
LocalPagamento=Pagável em qualquer agência bancária mesmo após o vencimento
Especie=DM
EspecieMod=R$
DataLimitePagto=
Sacado.NomeSacado =Sacado Teste
Sacado.CNPJCPF =999.999.999.
Sacado.Pessoa=
Sacado.Logradouro =Rua Jose Rodrigues
Sacado.Numero =
Sacado.Bairro =Jardim Moderno
Sacado.Complemento=Casa
Sacado.Cidade =Tatui
Sacado.UF =SP
Sacado.CEP =18277.
Sacado.Email=teste@email.com
Sacado.SacadoAvalista.Pessoa=
Sacado.SacadoAvalista.NomeAvalista=Nome do Avalista
Sacado.SacadoAvalista.CNPJCPF=
Sacado.SacadoAvalista.Logradouro=Rua das Flores
Sacado.SacadoAvalista.Numero=
```
27/10/24, 15:45 Modelo Titulo.INI

https://acbr.sourceforge.io/ACBrLib/ModeloTituloINI.html 1 / 2


```
Sacado.SacadoAvalista.Complemento=Casa
Sacado.SacadoAvalista.Bairro=Centro
Sacado.SacadoAvalista.Cidade=Tatui
Sacado.SacadoAvalista.UF=SP
Sacado.SacadoAvalista.CEP=
Sacado.SacadoAvalista.Email=teste@email.com
Sacado.SacadoAvalista.Fone=(99)
Sacado.SacadoAvalista.InscricaoNr=
Mensagem=teste1|teste
Informativo=teste1|teste2|teste3|teste
Detalhamento=Dados Fatura 1|Dados Fatura 2|Dados Fatura 3
Competencia=
ArquivoLogoEmp=
Verso=False
Instrucao1=
Instrucao2=
Instrucao3=
Aceite=
OcorrenciaOriginal.TipoOcorrencia=
Parcela=
TotalParcelas=
SeuNumero=
TipoDiasProtesto=
CodigoNegativacao=
TipoDiasNegativacao=
TipoImpressao=
CodigoMoraJuros=
CodigoMora=
TipoDesconto=
TipoDesconto2=
CarteiraEnvio=
QrCode.emv= ;;Obrigatório - Utilizado na modalidade Boleto Hibrido
QrCode.txid= ;;A depender do banco
QrCode.url= ;;A depender de banco
```
```
[NFe1-1] ;;Apenas para bancos que tem layout com informações de NFe. [NFe1-1] primeiro numero
corresponde ao Título | segundo número depois do traço (-) corresponde ao item NFe
NumNFe=
ValorNFe=
EmissaoNFe=
ChaveNFe=
```
```
Created with the Personal Edition of HelpNDoc: Free CHM Help documentation generator
(https://www.helpndoc.com)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:45 Modelo Titulo.INI

https://acbr.sourceforge.io/ACBrLib/ModeloTituloINI.html 2 / 2

ACBrLibBoleto (ACBrLibBoleto.html)/Informações (Informacoes1.html)/

# Modelo Cedente_Titulos.INI

[Cedente]
Nome=SAO JOAO LTDA.
CNPJCPF= 99.999.999/9999-
Logradouro=Rua Evaristo Mendes
Numero=
Bairro=Centro
Cidade=Tatui
CEP=18.270-
Complemento=Sala 10
UF=SP
RespEmis=
TipoPessoa=
CodigoCedente=
LayoutBol=
CaracTitulo=
TipoCarteira=
TipoDocumento=
Modalidade=
CodTransmissao=
Convenio=
Operacao=
PIX.TipoChavePix=
PIX.Chave=

[Conta]
Conta=
DigitoConta=
Agencia=
DigitoAgencia=
DigitoVerificadorAgenciaConta=

[Banco]
Numero=
CNAB=
TipoCobranca=
NumeroCorrespondente=
VersaoArquivo=
VersaoLote=

[Titulo1]
NumeroDocumento=
NossoNumero=
Carteira=
ValorDocumento=100,
Vencimento=10/09/
ValorMoraJuros=0,
DataDocumento=10/08/


DataProcessamento=10/08/
DataAbatimento=05/09/
DataDesconto=07/09/
DataMoraJuros=12/09/
DiasDeProtesto=
DataProtesto=10/10/
DataMulta=10/10/
ValorAbatimento=5,
ValorDesconto=0,
ValorMoraJuros=0,
ValorIOF=3,
ValorOutrasDespesas=2,
MultaValorFixo=
PercentualMulta=05,
LocalPagamento=Pagável em qualquer agência bancária mesmo após o vencimento
Especie=DM
EspecieMod=R$
Sacado.NomeSacado=Sacado Teste
Sacado.CNPJCPF=999.999.999.
Sacado.Pessoa=
Sacado.Logradouro=Rua Jose Rodrigues
Sacado.Numero=
Sacado.Bairro=Jardim Moderno
Sacado.Complemento=Casa
Sacado.Cidade=Tatui
Sacado.UF=SP
Sacado.CEP=18277.
Sacado.Email=teste@email.com
Sacado.SacadoAvalista.NomeAvalista=Nome do Avalista
Sacado.SacadoAvalista.CNPJCPF=
Sacado.SacadoAvalista.Logradouro=Rua das Flores
Sacado.SacadoAvalista.Numero=
Sacado.SacadoAvalista.Complemento=Casa
Sacado.SacadoAvalista.Bairro=Centro
Sacado.SacadoAvalista.Cidade=Tatui
Sacado.SacadoAvalista.UF=SP
Sacado.SacadoAvalista.CEP=
Sacado.SacadoAvalista.Email=teste@email.com
Sacado.SacadoAvalista.Fone=(99)
Sacado.SacadoAvalista.InscricaoNr=
Mensagem=teste1|teste
Informativo=teste1|teste2|teste3|teste
Instrucao1=
Instrucao2=

## Aceite=

## OcorrenciaOriginal.TipoOcorrencia=

## Parcela=

## TotalParcelas=

SeuNumero=

## TipoDiasProtesto=

## TipoImpressao=

CodigoMoraJuros=


## CodigoMora=

## TipoDesconto=

## TipoDesconto2=

[Titulo2]
NumeroDocumento=
NossoNumero=
Carteira=
ValorDocumento=100,
Vencimento=10/09/
ValorMoraJuros=0,
DataDocumento=10/08/
DataProcessamento=10/08/
DataAbatimento=05/09/
DataDesconto=07/09/
DataMoraJuros=12/09/
DiasDeProtesto=
DataProtesto=10/10/
DataMulta=10/10/
ValorAbatimento=5,
ValorDesconto=0,
ValorMoraJuros=0,
ValorIOF=3,
ValorOutrasDespesas=2,
MultaValorFixo=
PercentualMulta=05,
LocalPagamento=Pagável em qualquer agência bancária mesmo após o vencimento
Especie=DM
EspecieMod=R$
Sacado.NomeSacado=Sacado Teste
Sacado.CNPJCPF=999.999.999.
Sacado.Pessoa=
Sacado.Logradouro=Rua Jose Rodrigues
Sacado.Numero=
Sacado.Bairro=Jardim Moderno
Sacado.Complemento=Casa
Sacado.Cidade=Tatui
Sacado.UF=SP
Sacado.CEP=18277.
Sacado.Email=teste@email.com
Sacado.SacadoAvalista.NomeAvalista=Nome do Avalista
Sacado.SacadoAvalista.CNPJCPF=
Sacado.SacadoAvalista.Logradouro=Rua das Flores
Sacado.SacadoAvalista.Numero=
Sacado.SacadoAvalista.Complemento=Casa
Sacado.SacadoAvalista.Bairro=Centro
Sacado.SacadoAvalista.Cidade=Tatui
Sacado.SacadoAvalista.UF=SP
Sacado.SacadoAvalista.CEP=
Sacado.SacadoAvalista.Email=teste@email.com
Sacado.SacadoAvalista.Fone=(99)
Sacado.SacadoAvalista.InscricaoNr=


## Mensagem=teste1|teste

## Created with the Personal Edition of HelpNDoc: Qt Help documentation made easy

(https://www.helpndoc.com/feature-tour/create-help-files-for-the-qt-help-framework)

- Mensagem=teste1|teste
- Informativo=teste1|teste2|teste3|teste
- Instrucao1=
- Instrucao2=
- Aceite=
- OcorrenciaOriginal.TipoOcorrencia=
- Parcela=
- TotalParcelas=
- SeuNumero=
- TipoDiasProtesto=
- TipoImpressao=
- CodigoMora=
- TipoDesconto=
- TipoDesconto2=

ACBrLibBoleto (ACBrLibBoleto.html)/Informações (Informacoes1.html)/

# Indice de Códigos Titulo.INI

## Índice de Códigos utilizados no arquivo Titulo.INI

```
Neste tópico você vai encontrar todas os Códigos utilizados no preenchimento do arquivo Titulo.INI
```
Obs: Para ver os Índices de Códigos utilizados no arquivo Cedente.INI veja em: Configurações da Biblioteca
(ConfiguracoesdaBiblioteca18.html)

```
Índice Códigos
```
```
CHAVE DESCRIÇÃO
```
```
Sacado.Pessoa
```
```
Define Sacado como pessoa Física, Jurídica ou outras:
```
```
0 - Pessoa Física
1 - Pessoa Jurídica
2 - Outras
3 - Nenhum (utilizado pelo Santander)
```
```
Aceite
```
```
Define o tipo de Aceite para o Boleto:
```
```
0 - Sim
1 - Não
```

**OcorrenciaOriginal** Define o código de Ocorrências:
Obs: Constantemente ocorrem atualizações na lista de ocorrências. Isso acontece,
por exemplo, por causa de bancos novos.
Portanto para garantir a sua tabela de códigos de remessa esteja correta, utilize o
método BOLETO.ListaOcorrencias ou também BOLETO.ListaOcorrenciasEX().
Abaixo algum dos valores:

```
0 - RemessaRegistrar
1 - RemessaBaixar
2 - RemessaDebitarEmConta
3 - RemessaConcederAbatimento
4 - RemessaCancelarAbatimento
5 - RemessaConcederDesconto
6 - RemessaCancelarDesconto
7 - RemessaAlterarVencimento
8 - RemessaAlterarVencimentoSustarProtesto
9 - RemessaProtestar
10 - RemessaSustarProtesto
11 - RemessaCancelarInstrucaoProtestoBaixa
12 - RemessaCancelarInstrucaoProtesto
13 - RemessaDispensarJuros
14 - RemessaAlterarNomeEnderecoSacado
15 - RemessaAlterarNumeroControle
16 - RemessaOutrasOcorrencias
17 - RemessaAlterarControleParticipante
18 - RemessaAlterarSeuNumero
19 - RemessaTransfCessaoCreditoIDProd
20 - RemessaTransferenciaCarteira
21 - RemessaDevTransferenciaCarteira
22 - RemessaDesagendarDebitoAutomatico
23 - RemessaAcertarRateioCredito
24 - RemessaCancelarRateioCredito
25 - RemessaAlterarUsoEmpresa
26 - RemessaNaoProtestar
27 - RemessaProtestoFinsFalimentares
28 - RemessaBaixaporPagtoDiretoCedente
29 - RemessaCancelarInstrucao
30 - RemessaAlterarVencSustarProtesto
31 - RemessaCedenteDiscordaSacado
32 - RemessaCedenteSolicitaDispensaJuros
33 - RemessaOutrasAlteracoes
34 - RemessaAlterarModalidade
35 - RemessaAlterarExclusivoCliente
36 - RemessaNaoCobrarJurosMora
37 - RemessaCobrarJurosMora
38 - RemessaAlterarValorTitulo
39 - RemessaExcluirSacadorAvalista
40 - RemessaAlterarNumeroDiasProtesto
41 - RemessaAlterarPrazoProtesto
42 - RemessaAlterarPrazoDevolucao
43 - RemessaAlterarOutrosDados
44 - RemessaAlterarDadosEmissaoBloqueto
```

45 - RemessaAlterarProtestoDevolucao
46 - RemessaAlterarDevolucaoProtesto
47 - RemessaNegativacaoSerasa
48 - RemessaExcluirNegativacaoSerasa
49 - RemessaAlterarJurosMora
50 - RemessaAlterarMulta
51 - RemessaDispensarMulta
52 - RemessaAlterarDesconto
53 - RemessaNaoConcederDesconto
54 - RemessaAlterarValorAbatimento
55 - RemessaAlterarPrazoLimiteRecebimento
56 - RemessaDispensarPrazoLimiteRecebimento
57 - RemessaAlterarNumeroTituloBeneficiario
58 - RemessaAlterarDadosPagador
59 - RemessaAlterarDadosSacadorAvalista
60 - RemessaRecusaAlegacaoPagador
61 - RemessaAlterarDadosRateioCredito
62 - RemessaPedidoCancelamentoDadosRateioCredito
63 - RemessaPedidoDesagendamentoDebietoAutom
64 - RemessaAlterarEspecieTitulo
65 - RemessaAlterarContratoCobran
66 - RemessaNegativacaoSemProtesto
67 - RemessaBaixaTituloNegativadoSemProtesto
68 - RemessaAlterarValorMinimo
69 - RemessaAlterarValorMaximo
70 - RemessaExcluirNegativacaoSerasaBaixar
71 - RemessaExcluirNegativacaoManterEmCarteira
72 - RemessaSustarProtestoBaixarTitulo
73 - RemessaSustarProtestoManterCarteira
74 - RemessaRecusaAlegacaoSacado
75 - RemessaProtestoAutomatico
76 - RemessaAlterarStatusDesconto
77 - RemessaProtestarUrgente
78 - RemessaRegistrarDireta
79 - RemessaAlterarNumeroDiasBaixa
80 - RemessaAlterarValorMinimoMaximo
81 - RemessaAlteracaoQuantidadeParcela
82 - RemessaAlteracaoValorNominal
83 - RemessaNaoBaixarAutomaticamente
84 - RemessaAlteracaoPercentualParaMinimo
85 - RemessaAlteracaoPercentualParaMaximo
86 - RemessaAlteracaoPercentualParaMinimoMaximo
87 - RemessaProrrogarVencimento
88 - RemessaAlteracaoPercentualParaMinimoMaximo
89 - RemessaProrrogarVencimento
90 - RemessaHibrido

Caso nenhum desses valores seja passado, será assumido como valor default 0


```
TipoDiasProtesto
```
```
Define o tipo de contagem de dias para protesto:
```
```
0 - Dias corridos
1 - Dias úteis
```
```
TipoImpressao
```
```
Define o tipo de impressão de Boleto:
```
```
0 - Carnê
1 - Padrão
```
```
TipoDesconto ou
TipoDesconto
```
```
Define o tipo de desconto aceito pelo Banco:
```
```
0 - NaoConcederDesconto
1 - ValorFixoAteDataInformada
2 - PercentualAteDataInformada
3 - ValorAntecipacaoDiaCorrido
4 - ValorAntecipacaoDiaUtil
5 - PercentualSobreValorNominalDiaCorrido
6 - PercentualSobreValorNominalDiaUtil
7 - CancelamentoDesconto
```
```
CodigoMora
```
```
Define uma String com as orientações do Banco para ser impresso no Boleto:
```
```
1 - Valor Diário
2 - Taxa % Mensal
```
```
CodigoNegativacao
```
```
Define o Código para Negativação e Protesto utilizado por alguns Bancos:
```
```
0 - Nenhum
1 - ProtestarCorrido
2 - ProtestarUteis
3 - NaoProtestar
4 - Negativar
5 - NaoNegativar
6 - Cancelamento
```
```
Valores válidos para o
campo PIX.TipoChavePix
```
```
0 - Nenhuma
1 - Email
2 - CPF
3 - CNPJ
4 - Celular
5 - Aleatória
```
```
CodigoMoraJuros
```
```
0 - ValorDia
1 - TaxaMensal
2 - Isento
3 - ValorMensal,
4 - TaxaDiaria
```
```
Created with the Personal Edition of HelpNDoc: Full-featured EPub generator (https://www.helpndoc.com/create-
epub-ebooks)
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>

## ACBrLibBoleto (ACBrLibBoleto.html)/Informações (Informacoes1.html)/

# Particularidades

**Guia ACBrBoleto – Especificidades dos Bancos**

Este documento tem por finalidade orientar os usuários do ACBrBoleto quanto ao correto uso das propriedades que são particularidades de alguns bancos.

**1. Tabela com principais campos do grupo ACBrBoleto.Cedente e quais bancos os utilizam.**

```
Componente Monitor/ Lib BradescoBanco
do
Brasil
```
```
Banco da
Amazonia
```
```
BanestesItauSicrediMercantilCaixaCaixa
(Sicob)
```
```
HSBCBanco
Nordeste
```
```
BRBBICSafraDaycovalPineCecred
```
```
Agencia/DV Agencia/DigitoAgencia X X X X X X X X X X X X X X X X X
Conta/DV Conta/DigitoConta X X X X X X X X X X X X X X X X X
Endereço¹ Logradouro/Numero/Bairro/Cidade/CEP/UFX X X X X X X X X X X X X X X X X
CaracTitulo² CaracTitulo X X X X X X
Tipo Inscricao TipoPessoa X X X X X X X X X X X X X X X X X
CNPJ(CPF) CNPJCPF X X X X X X X X X X X X X X X X X
Telefone¹ Não Implementado X X X X X X X X X X X X X X X X X
Cod. Cedente Codigo
Cedente
```
### X X X X X X X X X X X

```
Cod.
Transmissão
```
```
Cod Transmissão X
```
```
Convenio Convenio X X X X X X
DV Agencia
Conta
```
```
DigitoVerificadorAgenciaConta X
```
```
Fantasia¹ Não Implementado X X X X X X X X X X
IdentDistribuicaoNão Implementado
Modalidade Modalidade X X X X X X X
Operacao Não Implementado X
Respon
Emissao
```
```
RespEmis X X X X X X X X X
```
```
TipoCarteira TipoCarteira X X
Tipo
Documento
```
```
Tipo
Documento
```
### X X X

```
Componente Monitor/ Lib Uniprime
XX
```
```
Unicred
XX
```
```
Banese Credsis Cresol CitiBank ABC
Brasil
```
```
Bancoob Banrisul Santander
```
```
Agencia/DV Agencia/DigitoAgencia X X X X X X X X X X
Conta/DV Conta/DigitoConta X X X X X X X X X X
Endereço¹ Logradouro/Numero/Bairro/Cidade/CEP/UFX X X X X X X X X X
CaracTitulo² CaracTitulo X X X
Tipo Inscricao TipoPessoa X X X X X X X X X X
```

### CNPJ(CPF) CNPJCPF X X X X X X X X X X

Telefone¹ Não Implementado X X X X X X X X X X

Cod. Cedente CodigoCedente X X X X

Cod. Transmissão CodTransmissão X X

Convenio Convenio X X

DV Agencia ContaDigitoVerificadorAgenciaConta X

Fantasia¹ Não Implementado X X X X X X X X X X

IdentDistribuicao Não Implementado X

Modalidade Modalidade X X X

Operacao Não Implementado X X

ResponEmissao RespEmis X X X X X

TipoCarteira TipoCarteira X X

TipoDocumento TipoDocumento X X

```
Componente Monitor/ Lib
Alfa
```
```
Money
Plus
```
```
Banco
C
```
```
Banco
Rendimento
```
```
Banco
Inter
```
```
BS2 PenseBank
API
```
### BTG

```
Pactual
```
```
Banco
Original
```
```
VotorantinPefisa FibraIndustrial
do Brasil
Agencia/DV Agencia/DigitoAgencia X X X X X X X X X X X X X
Conta/DV Conta/DigitoConta X X X X X X X X X X X X X
Endereço¹ Logradouro/Numero/Bairro/Cidade/CEP/UFX X X X X X X X X X X X X
CaracTitulo² CaracTitulo
Tipo Inscricao TipoPessoa X X X X X X X X X X X X X
CNPJ(CPF) CNPJCPF X X X X X X X X X X X X X
Telefone¹ Não Implementado
Cod. Cedente CodigoCedente X X X X X X X X X
Cod. TransmissãoCodTransmissão X X
Convenio Convenio X X X
DV Agencia
Conta
```
```
DigitoVerificadorAgenciaConta X
```
```
Fantasia¹ Não Implementado
IdentDistribuicaoNão Implementado X
Modalidade Modalidade X
Operacao Não Implementado X X X
ResponEmissao RespEmis X X X
TipoCarteira TipoCarteira X X
TipoDocumento TipoDocumento X
```

```
Componente Monitor/ Lib
Bocom
BBM
```
### UY

```
Agencia/DV Agencia/DigitoAgencia X X
Conta/DV Conta/DigitoConta X X
Endereço¹ Logradouro/Numero/Bairro/Cidade/CEP/UFX X
CaracTitulo² CaracTitulo X X
Tipo Inscricao TipoPessoa X X
CNPJ(CPF) CNPJCPF X X
Telefone¹ Não Implementado X X
Cod. Cedente CodigoCedente X X
Cod. TransmissãoCodTransmissão
Convenio Convenio
DV Agencia
Conta
```
```
DigitoVerificadorAgenciaConta
```
```
Fantasia¹ Não Implementado
IdentDistribuicao Não Implementado
Modalidade Modalidade
Operacao Não Implementado
ResponEmissao RespEmis
TipoCarteira TipoCarteira
TipoDocumento TipoDocumento
```
**Correspondentes**

**Componente Monitor/ Lib Banco do Brasil
Sicoob**

```
Safra Bradesco Pine
Bradesco
```
```
Bradesco
Sicoob
```
```
Banco Sofisa
Itau
```
```
Banco Athena
Bradesco
```
```
Banco
Pensebank
```
Agencia/DV Agencia/DigitoAgencia X X X X X X X

Conta/DV Conta/DigitoConta X X X X X X

Endereço¹ Logradouro/Numero/Bairro/Cidade/CEP/UFX X X X X X X

CaracTitulo² CaracTitulo X X X

Tipo Inscricao TipoPessoa X X X X X X X


### CNPJ(CPF) CNPJCPF X X X X X X X

```
Telefone¹ X X X X X X X X
Cod. Cedente CodigoCedente X X X
Cod. Transmissão CodTransmissão X X
Convenio Convenio X X X
DV Agencia Conta DigitoVerificadorAgenciaConta
Fantasia¹ Não Implementado X X X X
IdentDistribuicao Não Implementado
Modalidade Modalidade X
Operacao Não Implementado
ResponEmissao RespEmis X X X
TipoCarteira TipoCarteira
TipoDocumento TipoDocumento X
```
**2. Tabela com principais campos do grupo ACBrBoleto.Banco e quais bancos os utilizam.**

```
ComponenteMonitor/ Lib BradescoBanco do
Brasil
```
```
Banco da
Amazonia
```
```
BanestesItauSicrediMercantilCaixaCaixa
(Sicob)
```
```
HSBC Banco
Nordeste
```
```
BRBBIC SafraDaycoval Pine Cecred
```
```
Casas
Decimais
MoraJuros
```
```
Não Implementado X
```
```
Layout
Versao
Arquivo*
```
```
Versao
Arquivo
```
### X X X

```
Layout
VersaoLote*
```
```
VersaoLote X X X X X X X X X X
```
```
Local
Pagamento³
```
```
Local
Pagamento
```
### X X

```
ComponenteMonitor/ Lib Uniprime
XX
```
```
Unicred
XX
```
```
Banese Credsis Cresol CitiBank ABC Brasil Bancoob Banrisul Santander
```
```
Casas
Decimais
MoraJuros
```
```
Não
Implementado
```
### X

```
Layout
Versao
Arquivo*
```
```
Versao
Arquivo
```
### X X X

```
Layout
VersaoLote*
```
```
VersaoLote X X X
```
```
Local
Pagamento³
```
```
Local
Pagamento
```
### X X X X X X X X X X


```
Correspondentes
Componente Monitor/ Lib Banco do Brasil Sicoob Safra Bradesco Pine Bradesco Bradesco Sicoob
CasasDecimaisMoraJuros Não Implementado
LayoutVersaoArquivo* VersaoArquivo
LayoutVersaoLote* VersaoLote
LocalPagamento³ LocalPagamento X X X X
NumeroCorrespondente³ NumeroCorrespondente X X X X
```
**¹** Informações utilizadas somente para impressão do boleto

**²** Propriedade que poder informada tanto no cedente, quanto no titulo, se informado no cedente o titulo herdará o mesmo valor.

**³** Componente atribui valor default conforme regras dos bancos.

**3. Outras Informações Importantes**

**Obs.:** **_Para Integração Bancária por WebService ou API, consulte o tópico abaixo para saber os bancos com essa disponibilidade e os campos específicos para integração WEB._**
https://www.projetoacbr.com.br/forum/topic/57991-acbrboleto-via-webservice/ (https://www.projetoacbr.com.br/forum/topic/57991-acbrboleto-via-webservice/)

**3.1 Banco do Brasil**

ACBrBoleto.Banco.LayoutVersaoArquivo: Informar a versão do layout sendo utilizado, assume valor default caso nada seja informado.

ACBrBoleto.Cedente.Convenio: deve-se informar o convênio sem 0 a esquerda, pois junto com a carteira determina a quantidade de digitos livres para uso no nosso número.

Modalidade: Informar o valor chamado de variação pelo banco.

DataLimitePagto: esse campo é utilizado para cálculo dos dias para recebimento após vencimento.

**3.2 Banestes**

Modalidade: Tipo de cobrança informado pelo banco, com valores possíveis conforme manual do banco (2, 3, 4, 5, 6 e 7), usado para montar o campo AsBace.

**3.3 Sicredi**

ACBrTitulo.ACBrBoleto.Cedente.AgenciaDigito: Valor informado pelo banco como Posto Beneficiário, com 2 digitos.

Modalidade: Tipo de cobrança, 1- Com Registro ou diferente de 1 -Sem registro (atualmente em vigor somente cobrança com registro).

Titulo[x].CodigoGeração: Valor definido pelo banco como sendo o Byte de geração.

Titulo[x].CodigoMora: A- Valor ou B-Percentual.

Titulo[x].Informativo: Stringlist para envio de texto a ser impresso no boleto quando o mesmo é feito pelo banco.


Quando o banco gerar nosso número, informar 600 na propriedade CodigoGeracao e RespEmis = BancoEmite
Titulo[x].CodigoGeracao := '600';
ACBrBoleto.Cedente.RespEmis = ACBrResponEmissao.tbBancoEmite;
Lembrete: Atualmente o banco esta retornando nosso numero com inicio 600, favor conferir se esta batendo nossoNumero quando criado por eles.

**3.4 Caixa Econômica Sicob**

Titulo[x].Carteira: Informar RG para cobrança registrada e SR para cobrança sem registro (em vigor somente a registrada)

Titulo[x].CarteiraEnvio: Informar TceCedente para emissão do boleto pelo beneficiário e TceBanco para emissão pelo banco.

**3.5 Caixa Econômica (SIGCB)**

ACBrBoleto.Cedente.Convenio: deve-se informar o convênio incluíndo o Código de Operação.

Titulo[x].Carteira: Informar CS- Carteira Simples (11), CR- Carteira Rápida(12), SR – Sem Registro(14) ou DE- Carteira Descontada. (SR- Sem Registro fora de vigor atualmente)

PARA CÓDIGO DE BENEFICIÁRIO ENTRE 000001 E 999999
Para versões do layout ‘101’ (Header de Arquivo) e ‘060’ (Header de Lote), alinhar à esquerda e preencher com ‘0’ à direita, na última posição.
Exemplo 1: Código do Beneficiário: 339578 então o layout será 101 e lote 060

PARA CÓDIGO DE BENEFICIÁRIO A PARTIR DE 1 100000
Utilizar somente as versões de layout ‘107’ (Header de Arquivo) e ‘067’ (Header de Lote) com alinhamento à direita.
Exemplo 3: Código do Beneficiário: 1 100123

### 3.6 HSBC

Titulo[x].Carteira: Informar CSB / 1 – Carteira Registrada ou CNR / 2 – Carteira Sem Registro. (Atualmente somente Carteira Registrada em vigor)

Titulo[x].ValorAbatimento: Além de informar aqui o valor do abatimento, a propriedade Titulo[x].OcorrenciaOriginal.Tipo deverá ser toRemessaConcederAbatimento ou toRemessaCancelarAbatimento.

Titulo[x].PercentualMulta: Além de informar o percentual de multa aqui, deverá ser informado também a propriedade Titulo[x].DataMoraJuros e em Titulo[x].Instrucao1 os códigos 15 ou 16, quando trata-se de
data definida para inicio da cobrança de multa.

Quando a multa for cobrada X dias após o vencimento, deverão ser informados os valores 22 (dias úteis e multa em valor), 73 (dias corridos e multa em percentual) ou 74 (dias úteis e multa em percentual) na
propriedade Titulo[x].Instrucao1.

Quando a multa for cobrada logo após o vencimento, a propriedade Titulo[x].Instrucao1 deverá receber o valor 24.

**3.7 Banco do Nordeste**

Titulo[x].Carteira: Informar 01- Cobrança Simples Escritural, 02- Cobrança Vinculada, 04-Cobrança Simples, 05- Cobrança Vinculada ou I-Cobrança Simplificada.

Cedente.CaracTitulo: Informar tcSimples para Cobrança Simples ou tcVinculada para cobrança vinculada.

Cedente.ResponEmissao: Informar tbBancoEmite para emissão pelo banco ou tbCliEmite para emissão pelo beneficiário.

**3.8 Banco BRB**


Titulo[x].DataLimitePagto, Titulo[x].DataProtesto: Devido as instruções de multa e juros ficarem alocadas na remessa nas mesmas posições relativas a Limite para Pagamento e Protesto, se houver sido
informado multa e juros, nem o Limite para Pagamento e nem o Protesto serão incluídos na remessa, se somente uma instrução tiver sido utilizada será incluído o Limite para Pagamento e se ambos as
instruções estiverem disponíveis, então serão informados

**3.9 Banco Safra**

Titulo[x].PercentualMulta: Para que este campo seja tratado corretamente pelo banco, deverá ser informado na propriedade Titulo[x].Instrucao1 o valor 16, relativo a instrução de multa.

Titulo[x].ValorAbatimento: Se informado multa, o mesmo não derá incluido na remessa, uma vez que neste banco são usadas as mesmas posições.

Banco Safra Bradesco

Titulo[x].CaracTitulo: Informe aqui a informação passada pelo banco como Código da Carteira, sendo tcSimples(1) ou tcVinculada(2).

**3.10 Cecred**

Titulo[x].CaracTitulo: Informe aqui a informação passada pelo banco como Código da Carteira, sendo: tcSimples (1), tcVinculada (2), tcCaucionada (3) ou tcDescontada (4).

**3.11 Banco ABC Brasil**

Cedente.IdentDistribuicao: Informar de quem é a responsabilidade de distriibuição dos boletos, tbBancoDistribui ou tbClienteDistribui.

Titulo[x].CaracTitulo: Informe aqui a informação passada pelo banco como Código da Carteira, sendo: tcSimples (1), tcCaucionada (3), tcVinculada (5) ou tcDescontada (4).

Titulo[x].DataProtesto: Somente será adicionada a remessa se não houver sido informada nenhuma informação a propriedade Titulo[x].Instrucao1.

Titulo[x].DataProtesto: Somente será adicionada a remessa se não houver sido informada nenhuma informação a propriedade Titulo[x].Instrucao1.

Titulo[x].Instrucao2: Informar 1, 2 ou 3 conforme opção para baixa ou devolução do titulo, se nada for informado será adicionado automaticamente o código para Não Baixar.

Titulo[x].InstrucaoX: Se alguma das instruções contiver o código 94, a primeira mensagem da lista de mensagens será incluída no registro do Tipo 1 e as demais no registro especifico para mensagens.

**3.12 UnicredES**

ACBrBoleto.Banco.LayoutVersaoLote: Informar “ **44** ” para que a remessa seja gerada com o valor “ **UNICRED** ” ou “ **944** ” para ter o valor “ **UNICRED DO BRASIL** ” no header do arquivo.

Validação “identificação de titulo caucionável” (posição 108 CNAB 240), informar as propriedades:
Banco.LayoutVersaoArquivo = 085
Se ACBrTitulo.CaracTitulo = tcCaucionada ele preenche na posição 108 “S”, caso seja diferente de tcCaucionada ele preenche com “N”

**3.13 Banco Itaú**

Para Protesto ou Negativação preencher os campos:


Titulo[x].CodigoNegativacao: Utilizar Código “7” para Negativação ou códigos para Protesto “1” ProtestoDiasCorrido, “2” ProtestoDiasUteis.

Titulo[x].DataProtestoNegativacao ou Titulo[x].DataProtesto

**3.14 Banco Inter**
Para o calculo do campo livre necessário para a construção do código de barras e linha digitavel, é necessário na propriedade ACBrBoleto.Cedente.CodigoCedente informar o Número da Operação informado
pelo banco Inter (Conta Digital > Emissão via CNAB > Retorno).

**DataLimitePgto** Obrigatorio a data limite de pagamento ser menor ou igual a 60 dias

**Carteira 112:** Necessário registrar primeiro a remessa para obter o nosso número de posse do nosso número é possível realizar a impressão da ficha de compensação

**Diferenças entre a carteira 110 e 112:**

Carteira **112** : Você precisa aguardar o retorno do banco para capturar o NossoNumero criado por eles (utiliza-se o seuNumero para que você possa identificar o retorno)
Carteira **110** : Você já envia o boleto com o NossoNumero, não depende do retorno do Inter como na carteira 112.

Para comunicação com a API, necessário no banco Inter alimentar as propriedades em WebService além dos campos tradicionais ClientID, ClientSecret :

ArquivoCRT = Caminho e arq CRT ('C:\INTER\InterAPI_Certificado.crt')
ArquivoKEY = Caminho e arq Key ('C:\INTER\InterAPI_Chave.key')
Scope = (conforme manual/documentação)

**Atenção para quem quer utilizar boleto híbrido:**
É necessário você salvar a informação de retorno da propriedade “ **NossoNumeroCorrespondente** ” que é devolvida após a inclusão.
Esta propriedade é necessária para realizar as consultas, alterações e baixas na API Cobrança Inter PIX
Para saber mais sobre este novo endpoint, clique aqui (https://www.projetoacbr.com.br/forum/topic/77529-boas-not%C3%ADcias-banco-inter-agora-emite-boleto-h%C3%ADbrido/)

**Quando API Pix não está devolvendo NossoNumero** :
Existem relatos que após a inclusão , a API não está devolvendo o campo nossoNumero, neste cado se olhar o log, o banco está devolvendo: " **situacao** ": "EM_PROCESSAMENTO";
Então deve aguardar alguns minutinhos e realizar a consulta detalhe utilizando a propriedade **NossoNumeroCorrepondente**

Saiba Como configurar, clique aqui (https://www.projetoacbr.com.br/forum/topic/57991-acbrboleto-via-webservice/?do=findComment&comment=458837&_rid=1706)

**3.15 Banco BS**

Atualmente existem 02 (dois) layout’s de Remessa – registro Header (duas versões de manuais)

Para a versão de layout menor que 006, o resultado do nosso número de verificação (DV) será diferente. Para versões iguais ou maiores que 006, o resultado será sempre 0. Já para versões menores que 006, o
resultado do DV será 1, sempre quando ele for igual a 10 ou 11.

Para garantir que seu sistema esteja configurado corretamente, é importante que a propriedade LayoutVersaoArquivo esteja devidamente parametrizada.

**3.16 Banco Bancoob/ Sicoob**

Atenção com os preenchimentos dos dados.
No campo “Digito da agência” informar o Número do Posto.
No campo “Agência” informar o Cooperativa.

Para API, as chaves pode ser exportadas desta forma:
https://www.projetoacbr.com.br/forum/topic/73380-exportar-certificado-pem-crt-e-key/ (https://www.projetoacbr.com.br/forum/topic/73380-exportar-certificado-pem-crt-e-key/)


**3.17 Banco Santander**

Necessário o código de transmissão fornecido pelo banco.
Carteira, exemplo : 05, 06, 04
Modalidade, exemplo: 101,102,

**Atenção**
Para que a solução ACBrBoleto crie o DV do nossoNumero automaticamente deixe a propriedade sem preencher:
(CNAB) VersaoDF =
Para não criar o DV do nossoNumero:
(API) VersaoDF = V

**API Santander**
Quem utiliza a API, se for realizar testes não utilizar SandBox, utilizar testes no ambiente de Homologação.
Mais informações, veja este link:
https://www.projetoacbr.com.br/forum/topic/76632-altera%C3%A7%C3%A3o-do-endpoint-api-santander-para-testes/ (https://www.projetoacbr.com.br/forum/topic/76632-altera%C3%A7%C3%A3o-do-
endpoint-api-santander-para-testes/)

**3.18 Banco MoneyPlus**

Existem 2 manuais de enviou, ou seja, 2 (dois) tipos de remessa diferentes.
Para utilizar Layout novo da Grafeno, informar a propriedade LayoutVersaoArquivo = 2 ;
LayoutVersaoArquivo diferente de 2, é assumido Layout da XP Investimentos.

**3.19 Banco Mercantil**

No Banco Mercantil existe uma particularidade na composição do “Nosso Número” onde eles pedem para inciar com um número especifico do beneficiário.
Exemplo: eles informaram que precisa iniciar com “30”
Então na propriedade “Modalidade” você deve informar 30, ficando
Modalidade = 30

**3.20 Banco Athena Bradesco**

No Banco Athena Bradesco CNAB 400 informar os dados referente a NFe

Exemplo Delphi/Lazarus:
DadosNota := FACBrBoleto.CriarTituloNaLista.CriarNFeNaLista;
DadosNota.NumNFe := '001';
DadosNota.ValorNFe := 100.00;
DadosNota.EmissaoNFe := 01/11/2023;
DadosNota.ChaveNFe := '1233332228881 100010355221 1230912751230003950';

Exemplo INI para ACBrMonitor ou ACBrLibBoleto:
[NFe1-1]
NumNFe='001'
ValorNFe=100.
EmissaoNFe=01/11/
ChaveNFe='1233332228881 100010355221 1230912751230003950'

**3.21 Banco Daycoval**

No Banco Daycoval existem até o momento 3 (Três) versões de layouts diferentes, então é necessário determinar a propriedade LayOutVersãoLote com um dos valores da tabela abaixo:

ACBrBoleto.Banco.LayoutVersaoLote = 3 (quando o código de remessa citado no manual for igual a 3)
ACBrBoleto.Banco.LayoutVersaoLote = 4 (quando o código de remessa citado no manual for igual a 4)


ACBrBoleto.Banco.LayoutVersaoLote = 6 (quando o código de remessa citado no manual for igual a 6 - Padrão)

**3.22 Banco Banrisul**

Existe Layout atual 103 e anterior.
No Layout 103, CNAB 240 – Para sair 2 no Segmento P posição 62, informar a propriedade IdentDistribuicao=1 (0=tbBancoDistribui, 1= tbClienteDistribui)

## Created with the Personal Edition of HelpNDoc: Easily create EBooks (https://www.helpndoc.com/feature-tour)

## Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>

```
ACBrLibBoleto (ACBrLibBoleto.html)/
```
# Métodos da Biblioteca

```
Consulte os métodos exportados pela biblioteca.
```
```
Boleto_Método[( param1 [,param2, param3, paramN...])]
```
```
Parâmetros entre chaves '[' são opcionais.
```
```
param1, param2, paramN: Parâmetros necessários para a execução do comando. Os parâmetros podem ser
dos seguintes tipos:
Texto ou “String”: Para especificar "Strings" nos parâmetros use sempre aspas duplas (");
Notas: Para quebra de linha em "Strings" grandes, como a Observação no rodapé dos cupons,
use o sinal Pipe (|) e para especificar aspas dentro da String, use 2 aspas.
Exemplos válidos:
"DESCRICAO DO PRODUTO";
"Cano de 8"" polegadas" (exemplo com aspas internas);
```
```
Numéricos: Para especificar números nos parâmetros, não use aspas. Para separar as casas decimais
use o ponto (.). Não use separador de milhar ou símbolo de moeda (R$);
Exemplos válidos:
10
10.
0.
1234.
```
```
Booleano: Utilize 1 para verdadeiro e 0 para falso;
Created with the Personal Edition of HelpNDoc: Free EBook and documentation generator
(https://www.helpndoc.com)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:46 Métodos da Biblioteca

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos da Biblioteca (MetodosdaBiblioteca18.html)/
```
# Boleto_Inicializar

```
Método usado para inicializar o componente para uso da biblioteca, este método recebe dois parâmetros do
tipo Strings, PAnsiChar no pascal.
```
```
Este método necessita sempre ser chamado antes de utilizar qualquer função da biblioteca.
```
```
Comando: Boleto_Inicializar([ eArqConfig, eChaveCrypt ]);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 eArqConfig String Sim Localização do arquivo INI, pode ser em branco neste caso o
ACBrLib vai criar um novo arquivo INI.
```
```
02 eChaveCrypt String Sim
```
```
Chave de segurança para criptografar as informações
confidencias, pode ser em branco neste caso será usado a senha
padrão.
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a biblioteca foi inicializada corretamente.
```
```
-1 Indica que houve falhas na inicialização da biblioteca.
```
```
-5 Indica que não foi possível localizar o arquivo INI informado.
```
```
-6 Indica que não foi possível encontrar o diretório do arquivo INI.
```
```
Created with the Personal Edition of HelpNDoc: Produce electronic books easily (https://www.helpndoc.com/create-
epub-ebooks)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos da Biblioteca (MetodosdaBiblioteca18.html)/
```
# Boleto_Finalizar

```
Método usado para remover o componente ACBrNFe e suas classes da memoria.
Este método necessita sempre ser chamado quando não for utilizar mais a biblioteca para não deixar
objetos na memória.
Comando: Boleto_Finalizar();
RETORNO
Valor Descrição
0 Indica que a biblioteca foi inicializada corretamente.
-2 Indica que houve falhas na finalização da biblioteca.
Created with the Personal Edition of HelpNDoc: Create cross-platform Qt Help files
```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos da Biblioteca (MetodosdaBiblioteca18.html)/
```
# Boleto_UltimoRetorno

```
Método usado retornar o ultimo retorno processado pela biblioteca.
```
```
Este método necessita ser chamado caso a string seja menor que o retorno ou para retornar a
descrição do erro.
```
```
Comando: Boleto_UltimoRetorno(sMensagem, ref esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 sMensagem String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html).
```
```
02 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html).
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a biblioteca foi inicializada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos da Biblioteca (MetodosdaBiblioteca18.html)/
```
# Boleto_Nome

```
Método que retornar o nome da biblioteca.
```
```
Comando: Boleto_Nome(sNome, ref esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 sNome String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html).
```
```
02 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html).
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos da Biblioteca (MetodosdaBiblioteca18.html)/
```
# Boleto_Versao

```
Método que retornar a versão da biblioteca.
```
```
Comando: Boleto_Versao(sVersao, ref esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 sVersao String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html).
```
```
02 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html).
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a biblioteca foi inicializada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Free EPub and documentation generator
(https://www.helpndoc.com)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:46 Boleto_Versao

https://acbr.sourceforge.io/ACBrLib/Boleto_Versao.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/
```
# Métodos de Configuração

```
BOLETO_ConfigLer (Boleto_ConfigLer.html)
BOLETO (Boleto_ConfigGravar.html)_ConfigGravar (Boleto_ConfigGravar.html)
BOLETO (Boleto_ConfigLerValor.html)_ConfigLerValor (Boleto_ConfigLerValor.html)
BOLETO (Boleto_ConfigGravarValor.html)_ConfigGravarValor (Boleto_ConfigGravarValor.html)
BOLETO_ConfigImportar (Boleto_ConfigGravarValor.html)
BOLETO_ConfigExportar (Boleto_ConfigGravarValor.html)
```
```
Created with the Personal Edition of HelpNDoc: Generate Kindle eBooks with ease
(https://www.helpndoc.com/feature-tour/create-ebooks-for-amazon-kindle)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:46 Métodos de Configuração

https://acbr.sourceforge.io/ACBrLib/MetodosdeConfiguracao18.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos de Configuração (MetodosdeConfiguracao18.html)/
```
# Boleto_ConfigLer

```
Método usado para ler a configuração da biblioteca do arquivo INI informado.
Comando: Boleto_ConfigLer([eArqConfig]);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eArqConfig String Sim Arquivo INI para ler, se informado vazio será usado o valorpadrão.
```
## RETORNO

```
Valor Descrição
0 Indica que a biblioteca foi inicializada corretamente.
-5 Indica que não foi possível localizar o arquivo INI informado.
-6 Indica que não foi possível encontrar o diretório do arquivo INI.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: Easily create EBooks (https://www.helpndoc.com/feature-tour)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:46 Boleto_ConfigLer

https://acbr.sourceforge.io/ACBrLib/Boleto_ConfigLer.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos de Configuração (MetodosdeConfiguracao18.html)/
```
# Boleto_ConfigGravar

```
Método usado para gravar a configuração da biblioteca no arquivo INI informado.
Comando: Boleto_ConfigGravar([eArqConfig]);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eArqConfig String Sim Arquivo INI para ler, se informado vazio será usado o valorpadrão.
```
## RETORNO

```
Valor Descrição
0 Indica que a biblioteca foi inicializada corretamente.
-5 Indica que não foi possível localizar o arquivo INI informado.
-6 Indica que não foi possível encontrar o diretório do arquivo INI.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: Easily create Web Help sites (https://www.helpndoc.com/feature-
tour)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:46 Boleto_ConfigGravar

https://acbr.sourceforge.io/ACBrLib/Boleto_ConfigGravar.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos de Configuração (MetodosdeConfiguracao18.html)/
```
# Boleto_ConfigLerValor

```
Método usado para ler um determinado item da configuração.
```
```
Comando: Boleto_ConfigLerValor(eSessao, eChave, sValor, esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 eSessao String Não Nome da sessão de configuração.
```
```
02 eChave String Não Nome da chave da sessão.
```
```
03 sValor String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
04 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a biblioteca foi inicializada corretamente.
```
```
-1 Indica que a biblioteca não foi inicializada.
```
```
-3 Indica que houve erro ao ler a configuração informada.
```
```
Nota:
Consulte as chave e as configurações no tópico Configurações da Biblioteca (ConfiguracoesdaBiblioteca.html).
```
```
Created with the Personal Edition of HelpNDoc: Create cross-platform Qt Help files
(https://www.helpndoc.com/feature-tour/create-help-files-for-the-qt-help-framework)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_ConfigLerValor

https://acbr.sourceforge.io/ACBrLib/Boleto_ConfigLerValor.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos de Configuração (MetodosdeConfiguracao18.html)/
```
# Boleto_ConfigGravarValor

```
Método usado para gravar um determinado item da configuração.
Comando: Boleto_ConfigGravarValor(eSessao, eChave, sValor);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eSessao String Não Nome da sessão de configuração.
02 eChave String Não Nome da chave da sessão.
03 sValor String Não Valor para ser gravado na configuração lembrando que o mesmodeve ser um valor string compatível com a configuração.
```
## RETORNO

```
Valor Descrição
0 Indica que a biblioteca foi inicializada corretamente.
-1 Indica que a biblioteca não foi inicializada.
-3 Indica que houve erro ao ler a configuração informada.
Nota:
Consulte as chave e as configurações no tópico Configurações da Biblioteca (ConfiguracoesdaBiblioteca.html).
Created with the Personal Edition of HelpNDoc: Easily create Qt Help files (https://www.helpndoc.com/feature-tour)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_ConfigGravarValor

https://acbr.sourceforge.io/ACBrLib/Boleto_ConfigGravarValor.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos de Configuração (MetodosdeConfiguracao18.html)/
```
# Boleto_ConfigImportar

```
Método usado para importar a configuração da biblioteca do arquivo INI informado.
Comando: Boleto_ConfigImportar([eArqConfig]);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eArqConfig String Sim Arquivo INI para ler, se informado vazio será usado o valorpadrão.
```
## RETORNO

```
Valor Descrição
0 Indica que a biblioteca foi inicializada corretamente.
-5 Indica que não foi possível localizar o arquivo INI informado.
-6 Indica que não foi possível encontrar o diretório do arquivo INI.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: Free EPub and documentation generator
(https://www.helpndoc.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_ConfigImportar

https://acbr.sourceforge.io/ACBrLib/Boleto_ConfigImportar.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos de Configuração (MetodosdeConfiguracao18.html)/
```
# Boleto_ConfigExportar

```
Método usado para exportar a configuração da biblioteca do arquivo INI informado.
```
```
Comando: Boleto_ConfigExportar(sMensagem, ref esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 sMensagem String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html).
```
```
02 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html).
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a biblioteca foi inicializada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Single source CHM, PDF, DOC and HTML Help creation
(https://www.helpndoc.com/help-authoring-tool)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_ConfigExportar

https://acbr.sourceforge.io/ACBrLib/Boleto_ConfigExportar.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_ConfigurarDados

```
Método responsável por Alterar as Configurações do Cedente, Banco e Conta utilizando um arquivo .INI
obs: Os dados do Cedente também podem ser configurados utilizando a biblioteca do componente. veja
em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html)
IMPORTANTE: As informações do Cedente passadas através deste método não atualizam as
configurações da Biblioteca ( Configurações da Biblioteca ) (ConfiguracoesdaBiblioteca18.html), ou seja, servirá
apenas para o(s) titulo(s) atuais (em memória), que estão sendo atualizados no Boleto. Ao gravar as configurações
da lib, (Boleto_ConfigGravar), volta a prevalecer os dados configurados na Biblioteca "ACBrLib.ini".
```
```
Comando: Boleto_ConfigurarDados(eArquivoIni);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 eArquivoIni String Não Arquivo Cedente no formato ini do ACBr.
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Obs.: Modelo Cedente.INI (ModeloCedenteINI.html)
```
```
Created with the Personal Edition of HelpNDoc: Easy EBook and documentation generator
(https://www.helpndoc.com)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_ConfigurarDados

https://acbr.sourceforge.io/ACBrLib/Boleto_ConfigurarDados.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_IncluirTitulos

```
Método responsável por Incluir os Títulos utilizando um arquivo .INI.
```
```
Comando: Boleto_IncluirTitulos(eArquivoIni, [eTipoSaida]);
```
```
obs: Podem ser adicionados todos os Títulos do Cedente em um único arquivo, adicionando número
sequencial nas chaves.
ex:
[Titulo1]
...
[Tutulo2]
...
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 eArquivoIni String Não Arquivo Titulos no formato ini do ACBr.
```
```
02 eTipoSaida String Sim
```
```
Se informado o tipo de Saída será executado a tarefa conforme
solicitação abaixo:
P - PDF
I - Impressora
E - e-mail
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Obs.: Modelo Titulo.INI (ModeloTituloINI.html)
Alterações na ACBrLibBoleto (https://www.projetoacbr.com.br/forum/topic/62964-altera%C3%A7%C3%B5es-
na-acbrlibboleto/)
(Altera%C3%A7%C3%B5es%20na%20ACBrLibBoleto)
```
```
Created with the Personal Edition of HelpNDoc: Produce online help for Qt applications
(https://www.helpndoc.com/feature-tour/create-help-files-for-the-qt-help-framework)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_IncluirTitulos

https://acbr.sourceforge.io/ACBrLib/Boleto_IncluirTitulos.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_Imprimir

```
Método para impressão dos Boletos adicionados na Lista.
Comando: Boleto_Imprimir([eNomeImpressora]);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eNomeImpressora String Sim String com nome exato da impressora instalada, paraimpressão.
```
## RETORNO

```
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: Generate Kindle eBooks with ease
(https://www.helpndoc.com/feature-tour/create-ebooks-for-amazon-kindle)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_Imprimir

https://acbr.sourceforge.io/ACBrLib/Boleto_Imprimir.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_ImprimirBoleto

```
Método para impressão individual de Boleto da Lista.
Comando: Boleto_ImprimirBoleto(eIndice, [eNomeImpressora]);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eIndice Integer Não Índice do Titulo na lista a ser impresso (Inicia com 0).
02 eNomeImpressora String Sim String com nome exato da impressora instalada, paraimpressão.
```
## RETORNO

```
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: What is a Help Authoring tool?
(https://www.helpauthoringsoftware.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_ImprimirBoleto

https://acbr.sourceforge.io/ACBrLib/Boleto_ImprimirBoleto.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_GerarRemessa

```
Método responsável por Gerar o arquivo de Remessa dos Títulos adicionados a Lista.
Comando: Boleto_GerarRemessa([eDirArqRemessa], [NumeroArquivo], [eNomeArquivo]);
obs: As informações de Diretório e Nome de Arquivo também podem ser configurados utilizando a biblioteca
do componente. veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html).
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eDirArqRemessa String Sim Diretório para geração do arquivo de remessa.
02 NumeroArquivo Integer Sim Numero Sequencial do arquivo.
03 eNomeArquivo String Sim Nome do Arquivo.
```
```
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: What is a Help Authoring tool?
(https://www.helpauthoringsoftware.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_GerarRemessa

https://acbr.sourceforge.io/ACBrLib/Boleto_GerarRemessa.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_GerarRemessaStream

```
Método responsável por Gerar o arquivo de Remessa dos Títulos adicionados a Lista em formato Base64.
Comando: Boleto_GerarRemessa([NumeroArquivo], sResposta, esTamanho);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 NumeroArquivo Integer Sim Numero Sequencial do arquivo.
02 sResposta String Não Usado pelo retorno, contem as informações retornadas.
03 esTamanho Integer Não Usado pelo retorno, contem o tamanho da string (sResposta).
```
```
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Produce electronic books easily (https://www.helpndoc.com/create-
epub-ebooks)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:47 Boleto_GerarRemessaStream

https://acbr.sourceforge.io/ACBrLib/Boleto_GerarRemessaStream.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_LerRetorno

```
Método responsável pela Leitura do arquivo de Retorno e popular os campos lidos na lista de Títulos.
Comando: Boleto_LerRetorno([eDirArqRemessa], [eNomeArquivo]);
obs: As informações de Diretório e Nome de Arquivo também podem ser configurados utilizando a biblioteca
do componente. veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html).
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eDirArqRetorno String Sim Diretório para leitura do arquivo Retorno.
02 eNomeArquivo String Sim Nome do Arquivo.
```
```
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: Free EBook and documentation generator
(https://www.helpndoc.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:48 Boleto_LerRetorno

https://acbr.sourceforge.io/ACBrLib/Boleto_LerRetorno.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_LerRetornoStream

```
Método responsável pelo processamento da stream do arquivo de retorno.
Comando: Boleto_LerRetornoStream(ARetornoBase64, sResposta, esTamanho);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 ARetornoBase64 String Não Stream do arquivo de retorno
02 sResposta String Não Usado pelo retorno, contem as informações retornadas.
03 esTamanho Integer Não Usado pelo retorno, contem o tamanho da string (sResposta).
```
```
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
## W0NFREVOVEVdDQpDTlBKQ1BGPQ0KTm9tZT1GTE9SRU5DSU8gTUVMTyBMVERBIE1FDQpGYW50YXNpYUNlZGVudGU9DQpMb2dyYWRvdXJvPQ

```
Created with the Personal Edition of HelpNDoc: Free iPhone documentation generator (https://www.helpndoc.com/feature-tour/iphone-website-generation)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
## 27/10/24, 15:48 Boleto_LerRetornoStream

## https://acbr.sourceforge.io/ACBrLib/Boleto_LerRetornoStream.html 1 / 1

ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/

# Boleto_ObterRetorno

```
Método responsável pela Leitura do arquivo de Retorno obtem a os dados de todos os títulos na resposta.
```
```
Comando: Boleto_LerRetorno([eDirArqRemessa], [eNomeArquivo], sResposta, esTamanho);
```
obs: As informações de Diretório e Nome de Arquivo também podem ser configurados utilizando a biblioteca
do componente. veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html).

```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 eDirArqRetorno String Sim Diretório para leitura do arquivo Retorno.
```
```
02 eNomeArquivo String Sim
```
```
Nome do Arquivo.
```
```
03 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
04 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```

## [CEDENTE]

Nome=Empresa Teste
CNPJCPF=12.345.678/9012-
CodigoCedente=
MODALIDADE=
CODTRANSMISSAO=
CONVENIO=

[BANCO]
Numero=
IndiceACBr=
NumeroCorrespondente=
VersaoArquivo=
VersaoLote=

[CONTA]
Conta=
DigitoConta=
Agencia=
DigitoAgencia=

[Titulo1]
Sacado.Nome=
Sacado.CNPJCPF=
Vencimento=29/06/
DataDocumento=30/12/
NumeroDocumento=NF 12345
DataProcessamento=06/06/
NossoNumero=
Carteira=
ValorDocumento=
DataOcorrencia=27/06/
DataCredito=28/06/
DataBaixa=29/06/
ValorDespesaCobranca=3,
ValorAbatimento=
ValorDesconto=
ValorMoraJuros=
ValorIOF=
ValorOutrasDespesas=
ValorOutrosCreditos=
ValorRecebido=
SeuNumero=NF 00548 12345
CodTipoOcorrencia=toRetornoLiquidado
DescricaoTipoOcorrencia=06-Liquidação

[MotivoRejeicao1-1]
MotivoRejeicao=04-Compensação Eletrônica.

[MotivoRejeicao1-2]
MotivoRejeicao=10-BaixaRejeitada


```
Created with the Personal Edition of HelpNDoc: Full-featured multi-format Help generator
(https://www.helpndoc.com/help-authoring-tool)
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_TotalTitulosLista

```
Método para retorno do Total de Títulos da Lista.
Comando: Boleto_TotalTitulosLista():
RETORNO
Valor Descrição
0+ Qualquer retorno positivo indica execução correta e o total.Ex.: Se retornar 1 o total de titulo é um, se for 0 o total é zero e assim por diante.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: Free PDF documentation generator (https://www.helpndoc.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:48 Boleto_TotalTitulosLista

https://acbr.sourceforge.io/ACBrLib/Boleto_TotalTitulosLista.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_LimparLista

```
Método para limpar os Títulos da Lista.
Comando: Boleto_LimparLista();
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Free iPhone documentation generator
(https://www.helpndoc.com/feature-tour/iphone-website-generation)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:48 Boleto_LimparLista

https://acbr.sourceforge.io/ACBrLib/Boleto_LimparLista.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_EnviarEmail

```
Método para envio de e-mail dos boletos adicionados a lista.
Comando: Boleto_EnviarEmail(ePara, [eAssunto], [eMensagem], [eCC]);
obs: As configurações para envio de email devem ser previamente configurados utilizando a biblioteca do
componente. veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html).
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 ePara String Não Endereço de e-mail para envio.
02 eAssunto String Sim Descrição do Assunto do e-mail.
03 eMensagem String Sim String com Mensagem no corpo do e-mail.
04 eCC String Sim Endereço de e-mail para cópia.
```
```
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Generate EPub eBooks with ease (https://www.helpndoc.com/create-
epub-ebooks)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:48 Boleto_EnviarEmail

https://acbr.sourceforge.io/ACBrLib/Boleto_EnviarEmail.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_EnviarEmailBoleto

```
Método para envio de e-mail dos boletos adicionados a lista.
Comando: Boleto_EnviarEmailBoleto(eIndice, ePara, [eAssunto], [eMensagem], [eCC]);
obs: As configurações para envio de email devem ser previamente configurados utilizando a biblioteca do
componente. veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html).
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eIndice Integer Não Índice do Titulo na lista a ser impresso (Inicia com 0).
02 ePara String Não Endereço de e-mail para envio.
03 eAssunto String Sim Descrição do Assunto do e-mail.
04 eMensagem String Sim String com Mensagem no corpo do e-mail.
05 eCC String Sim Endereço de e-mail para cópia.
```
```
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Easily create Help documents (https://www.helpndoc.com/feature-
tour)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:48 Boleto_EnviarEmailBoleto

https://acbr.sourceforge.io/ACBrLib/Boleto_EnviarEmailBoleto.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_SelecionaBanco

```
Método para selecionar Banco do Cedente, antes da Inclusão do Título.
Comando: Boleto_SelecionaBanco(CodBanco);
obs: Todas as configurações do cedente, assim como o Banco também podem ser previamente
configurados utilizando a biblioteca do componente. veja em: Configurações da Biblioteca
(ConfiguracoesdaBiblioteca18.html).
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 CodBanco String Não Código do banco a ser utilizado ex: 001.
```
```
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: What is a Help Authoring tool?
(https://www.helpauthoringsoftware.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:48 Boleto_SelecionaBanco

https://acbr.sourceforge.io/ACBrLib/Boleto_SelecionaBanco.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_GerarHTML

```
Método para geração dos Boletos adicionados a Lista em formato HTML.
Comando: Boleto_GerarHTM();
obs: As configurações do diretório para geração podem ser configurados utilizando a biblioteca do
componente. veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html)
ou utilizando o Método Boleto_SetDiretorioArquivo.
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Free HTML Help documentation generator
(https://www.helpndoc.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:48 Boleto_GerarHTML

https://acbr.sourceforge.io/ACBrLib/Boleto_GerarHTML.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_GerarPDF

```
Método para geração de PDF dos Boletos adicionados a Lista.
Comando: Boleto_GerarPDF();
obs: As configurações do diretório para geração podem ser configurados utilizando a biblioteca do
componente. veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html)
ou utilizando o Método Boleto_SetDiretorioArquivo.
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Free HTML Help documentation generator
(https://www.helpndoc.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:48 Boleto_GerarPDF

https://acbr.sourceforge.io/ACBrLib/Boleto_GerarPDF.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_SalvarPDF

```
Método para geração de PDF dos Boletos em formato Base64.
Comando: Boleto_SalvarPDF( sResposta, esTamanho );
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 sResposta String Não Usado pelo retorno, contem as informaçõesretornadas.
```
```
02 esTamanho Integer Não Usado pelo retorno, contem o tamanho dastring (sResposta).
```
## RETORNO

```
Valor Descrição
0 Indica que o método foi executado corretamente.
-1 Indica que a biblioteca não foi inicializada.
-10 Indica que houve erro ao executar a função.
Created with the Personal Edition of HelpNDoc: Easy EBook and documentation generator
(https://www.helpndoc.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:49 Boleto_SalvarPDF

https://acbr.sourceforge.io/ACBrLib/Boleto_SalvarPDF.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_GerarPDFBoleto

```
Método para geração de PDF dos Boletos adicionados a Lista.
Comando: Boleto_GerarPDFBoleto(eIndice);
obs: As configurações do diretório para geração podem ser configurados utilizando a biblioteca do
componente. veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html)
ou utilizando o Método Boleto_SetDiretorioArquivo.
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eIndice Integer Não Índice do Titulo na lista a ser impresso (Inicia com 0).
```
```
RETORNO
Valor Descrição
0 Indica que o método foi inicializada corretamente.
-1 Indica que a biblioteca não foi inicializada.
-10 Indica que houve erro ao gerar o PDF do evento.
Created with the Personal Edition of HelpNDoc: Easily create Help documents (https://www.helpndoc.com/feature-
tour)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:49 Boleto_GerarPDFBoleto

https://acbr.sourceforge.io/ACBrLib/Boleto_GerarPDFBoleto.html 1 / 1

```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_SalvarPDFBoleto

```
Método para geração de PDF dos Boletos em formato Base64.
Comando: Boleto_SalvarPDFBoleto(eIndice);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 eIndice Integer Não Índice do Titulo na lista a ser impresso (Inicia com 0).
```
```
RETORNO
Valor Descrição
0 Indica que o método foi inicializada corretamente.
-1 Indica que a biblioteca não foi inicializada.
-10 Indica que houve erro ao gerar o PDF do evento.
Created with the Personal Edition of HelpNDoc: Free Qt Help documentation generator (https://www.helpndoc.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:49 Boleto_SalvarPDFBoleto

https://acbr.sourceforge.io/ACBrLib/Boleto_SalvarPDFBoleto.html 1 / 1



```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_ListaBancos

```
Método para Listar os Bancos disponíveis no Componente ACBrLibBoleto.
Comando: Boleto_ListaBancos(sResposta, esTamanho);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 sResposta String Não String com tamanho predefinido para que a mesma possa ser preenchida com o valor de retorno, maisinformações em Como trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
02 esTamanho Integer Não Tamanho da string, inteiro que determina o tamanho da string passada no primeiro parâmetro, mais informaçõesem Como trabalhar com Strings? (ComotrabalharcomStrings.html)
```
### RETORNO

```
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Resposta
BancoDoBrasil|Santander|CaixaEconomica|CaixaSicob|Bradesco|Itau|BancoMercantil|Sicred|Bancoob|Banrisul|Banestes|HSBC|BancoDoNordeste|BRB|BicBanco|BradescoSICOO
Created with the Personal Edition of HelpNDoc: Free EPub and documentation generator (https://www.helpndoc.com)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
## 27/10/24, 15:49 Boleto_ListaBancos

## https://acbr.sourceforge.io/ACBrLib/Boleto_ListaBancos.html 1 / 1



```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_ListaCaractTitulo

```
Método para Listar as Características de Carteiras aceitas pelo componente.
```
```
Comando: Boleto_ListaCaractTitulo(sResposta, esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
02 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```
```
Simples|Vinculada|Caucionada|Descontada|Vendor
```
```
Created with the Personal Edition of HelpNDoc: Easily create Qt Help files (https://www.helpndoc.com/feature-tour)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:49 Boleto_ListaCaractTitulo

https://acbr.sourceforge.io/ACBrLib/Boleto_ListaCaractTitulo.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_ListaOcorrencias

```
Método para Listar os tipos de ocorrências aceito pelos Bancos.
Comando: Boleto_ListaOcorrencias(sResposta, esTamanho);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 sResposta String Não String com tamanho predefinido para que a mesma possa ser preenchida com o valor de retorno, maisinformações em Como trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
02 esTamanho Integer Não Tamanho da string, inteiro que determina o tamanho da string passada no primeiro parâmetro, mais informaçõesem Como trabalhar com Strings? (ComotrabalharcomStrings.html)
```
### RETORNO

```
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
RemessaRegistrar|RemessaBaixar|RemessaDebitarEmConta|RemessaConcederAbatimento|RemessaCancelarAbatimento|RemessaConcederDesconto|RemessaCancelarDescon
Created with the Personal Edition of HelpNDoc: Easily create HTML Help documents (https://www.helpndoc.com/feature-tour)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
## 27/10/24, 15:49 Boleto_ListaOcorrencias

## https://acbr.sourceforge.io/ACBrLib/Boleto_ListaOcorrencias.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_ListaOcorrenciasEX

```
Método para Listar os códigos e tipos de ocorrências aceito pelos Bancos.
```
```
Comando: Boleto_ListaOcorrenciasEX(sResposta, esTamanho);
```
```
obs: A listagem de Código retornado pode ser utilizada como índice para geração do título ou Identificação
da Ocorrência no Retorno. Campo = "OcorrenciaOriginal.TipoOcorrencia".
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
02 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```
```
0-RemessaRegistrar|1-RemessaBaixar|2-RemessaDebitarEmConta|3-RemessaConcederAbatimento|4-
RemessaCancelarAbatimento|5-RemessaConcederDesconto|6-RemessaCancelarDesconto|7-
RemessaAlterarVencimento|8-RemessaAlterarVencimentoSustarProtesto|9-RemessaProtestar|10-
RemessaSustarProtesto|11-RemessaCancelarInstrucaoProtestoBaixa|12-RemessaCancelarInstrucaoProtesto|13-
RemessaDispensarJuros|14-RemessaAlterarNomeEnderecoSacado|15-RemessaAlterarNumeroControle|16-
RemessaOutrasOcorrencias|17-RemessaAlterarControleParticipante|18-RemessaAlterarSeuNumero|19-
RemessaTransfCessaoCreditoIDProd10|20-RemessaTransferenciaCarteira|21-
RemessaDevTransferenciaCarteira|22-RemessaDesagendarDebitoAutomatico|23-
RemessaAcertarRateioCredito|24-RemessaCancelarRateioCredito|25-RemessaAlterarUsoEmpresa|26-
RemessaNaoProtestar|27-RemessaProtestoFinsFalimentares|28-RemessaBaixaporPagtoDiretoCedente|29-
RemessaCancelarInstrucao|30-RemessaAlterarVencSustarProtesto|31-RemessaCedenteDiscordaSacado|32-
RemessaCedenteSolicitaDispensaJuros|33-RemessaOutrasAlteracoes|34-RemessaAlterarModalidade|35-
RemessaAlterarExclusivoCliente|36-RemessaNaoCobrarJurosMora|37-RemessaCobrarJurosMora|38-
RemessaAlterarValorTitulo|39-RemessaExcluirSacadorAvalista|40-RemessaAlterarNumeroDiasProtesto|41-
RemessaAlterarPrazoProtesto|42-RemessaAlterarPrazoDevolucao|43-RemessaAlterarOutrosDados|44-
RemessaAlterarDadosEmissaoBloqueto|45-RemessaAlterarProtestoDevolucao|46-
RemessaAlterarDevolucaoProtesto|47-RemessaNegativacaoSerasa|48-RemessaExcluirNegativacaoSerasa|
```
27/10/24, 15:49 Boleto_ListaOcorrenciasEX

https://acbr.sourceforge.io/ACBrLib/Boleto_ListaOcorrenciasEX.html 1 / 2


```
Created with the Personal Edition of HelpNDoc: Create HTML Help, DOC, PDF and print manuals from 1 single source
(https://www.helpndoc.com/help-authoring-tool)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:49 Boleto_ListaOcorrenciasEX

https://acbr.sourceforge.io/ACBrLib/Boleto_ListaOcorrenciasEX.html 2 / 2


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_CodigosMoraAceitos

```
Método para Listar os códigos de Mora aceito pelos Bancos.
```
```
Comando: Boleto_CodigosMoraAceitos(sResposta, esTamanho);
```
```
obs: A listagem de Código retornado pode ser utilizada como índice para a geração do Título campo:
"CodigoMora".
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
02 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```
```
1 2
```
```
Created with the Personal Edition of HelpNDoc: Write eBooks for the Kindle (https://www.helpndoc.com/feature-
tour/create-ebooks-for-amazon-kindle)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:49 Boleto_CodigosMoraAceitos

https://acbr.sourceforge.io/ACBrLib/Boleto_CodigosMoraAceitos.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_SetDiretorioArquivo

```
Método para Configurar o Diretório para Geração de Boletos PDF ou HTML.
Comando: Boleto_SetDiretorioArquivo(sDiretorio, [sArquivo]);
obs: As informações de Diretório e Nome de Arquivo também podem ser configurados utilizando a biblioteca
do componente. Veja em: Configurações da Biblioteca (ConfiguracoesdaBiblioteca18.html).
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 sDiretorio String Não String com caminho do Diretório.
02 sArquivo String Sim String com Nome do Arquivo.
```
```
RETORNO
Valor Descrição
0 Indica que a função foi executada corretamente.
-10 Indica que houve falhas na execução do método.
```
```
Created with the Personal Edition of HelpNDoc: Full-featured EBook editor (https://www.helpndoc.com/create-epub-
ebooks)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:49 Boleto_SetDiretorioArquivo

https://acbr.sourceforge.io/ACBrLib/Boleto_SetDiretorioArquivo.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_TamNossoNumero

```
Método para Calcular o Tamanho do campo Nosso Número.
Comando: Boleto_TamNossoNumero(sCarteira, sNossoNumero, sConvenio);
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
01 sCarteira String Não String com numero da Carteira.
02 sNossoNumero String Não String com Nosso Numero.
03 sConvenio String Não String com número do Convênio.
```
```
RETORNO
Valor Descrição
0+ Qualquer retorno positivo indica execução correta e o tamanho.Ex.: Se retornar 1 o tamanho é um, se for 0 o tamanho é zero e assim por diante.
-10 Indica que houve falhas na execução do método.
Created with the Personal Edition of HelpNDoc: Create cross-platform Qt Help files
(https://www.helpndoc.com/feature-tour/create-help-files-for-the-qt-help-framework)
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:50 Boleto_TamNossoNumero

https://acbr.sourceforge.io/ACBrLib/Boleto_TamNossoNumero.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_MontarNossoNumero

```
Método para Calcular e Retornar o NossoNumero completo de acordo com o Banco Configurado.
```
```
Comando: Boleto_MontarNossoNumero(Indice, sResposta, esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 Indice Integer Não Indice do Titulo na lista a ser Calculado (Inicia com 0)
```
```
02 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
03 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```
```
21545600000-
```
```
Created with the Personal Edition of HelpNDoc: Easily create EBooks (https://www.helpndoc.com/feature-tour)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:50 Boleto_MontarNossoNumero

https://acbr.sourceforge.io/ACBrLib/Boleto_MontarNossoNumero.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_RetornarLinhaDigitavel

```
Método para Calcular e Retornar a Linha Digitável do Boleto.
```
```
Comando: Boleto_RetornarLinhaDigitavel(Indice, sResposta, esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 Indice Integer Não Indice do Titulo na lista a ser Calculado (Inicia com 0)
```
```
02 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
03 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```
```
00192.15458 60000.000087 68503.410109 7 72160000010050
```
```
Created with the Personal Edition of HelpNDoc: News and information about help authoring tools and software
(https://www.helpauthoringsoftware.com)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:50 Boleto_RetornarLinhaDigitavel

https://acbr.sourceforge.io/ACBrLib/Boleto_RetornarLinhaDigitavel.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_RetornaCodigoBarras

```
Método para Calcular e Retornar o Código de Barras do Boleto.
```
```
Comando: Boleto_RetornaCodigoBarras(Indice, sResposta, esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 Indice Integer Não Indice do Titulo na lista a ser Calculado (Inicia com 0)
```
```
02 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
03 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```
```
00197721600000100502154560000000086850341010
```
```
Created with the Personal Edition of HelpNDoc: iPhone web sites made easy (https://www.helpndoc.com/feature-
tour/iphone-website-generation)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:50 Boleto_RetornaCodigoBarras

https://acbr.sourceforge.io/ACBrLib/Boleto_RetornaCodigoBarras.html 1 / 1


```
ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/
```
# Boleto_EnviarBoleto

```
Método para Registro de Boleto online via WebService ou API.
É necessário utilizar o Boleto_IncluirTitulos para adicionar o Título antes do envio (caso Registrado com
êxito o Boleto poderá ser emitido, caso contrário validar as rejeições antes da emissão).
```
```
Obs.: Para Integração Bancária por WebService ou API, consulte o tópico abaixo para saber os
bancos com essa disponibilidade e as configurações específicas para integração WEB.
https://www.projetoacbr.com.br/forum/topic/57991-acbrboleto-via-webservice/
(https://www.projetoacbr.com.br/forum/topic/57991-acbrboleto-via-webservice/)
Lembre-se de configurar o log na seção [ BoletoWebSevice] facilita encontrar erros de comunicação com
webService/API, clique aqui. (ConfiguracoesdaBiblioteca18.html)
Comando: Boleto_EnviarBoleto(eCodigoOperacao, sResposta, esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 eCodigoOperacao Integer Não
```
```
Código da operação:
0 = tpInclui
1 = tpAltera
2 = tpBaixa
3 = tpConsulta
4 = tpConsultaDetalhe
5 = tpPIXCriar - obs: Operações com PIX apenas para API
Banco do Brasil
6 = tpPIXCancelar
7 = tpPIXConsultar
8 = tpCancelar
9 = tpTicket
```
```
02 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
03 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```
27/10/24, 15:50 Boleto_EnviarBoleto

https://acbr.sourceforge.io/ACBrLib/Boleto_EnviarBoleto.html 1 / 2


## [REGISTRO1]

```
CodRetorno=
ControleCodRetorno=
ControleData=
ControleHora=
ControleNSU=
ControleOriRetorno=
ControleRetorno=
Excecao=
Header_Agencia=
Header_Autenticacao=
Header_CNPJCPF_Beneficiario=
Header_Data_Hora=
Header_Id_Origem=
Header_Id_Processo=
Header_Indice=
Header_Operacao=INCLUI_BOLETO
Header_Sistema_Origem=
Header_Usuario=
Header_Usuario_Servico=
Header_Versao=
IDCodBarras=
IDLinhaDig=
IDNossoNum=
IDURL=
IndicadorContinuidade=
MsgRetorno=
OriRetorno=
ProximoIndice=
```
```
[REJEICAO1-1]
Campo=
Codigo=
Mensagem=
Ocorrencia=
Valor=
Versao=
```
```
Created with the Personal Edition of HelpNDoc: Easy EBook and documentation generator
(https://www.helpndoc.com)
```
```
Copyright © <2018-2021> por <ACBr - Automação Comercial Brasil>
```
27/10/24, 15:50 Boleto_EnviarBoleto

https://acbr.sourceforge.io/ACBrLib/Boleto_EnviarBoleto.html 2 / 2


ACBrLibBoleto (ACBrLibBoleto.html)/Métodos Boleto (MetodosBoleto.html)/

# Boleto_ConsultarTitulosPorPeriodo

Método para Consulta de Títulos por período via API (obs: Serviço disponível apenas para API Banco do
Brasil).

```
Comando: Boleto_ConsultarTitulosPorPeriodo(eArquivoIni, sResposta, esTamanho);
```
```
SEQ. NOME TIPO OPICIONAL DESCRIÇÃO
```
```
01 eArquivoIni String Não
```
```
Path ou arquivo .ini com os filtros. Exemplo do .ini:
```
```
[ConsultaAPI]
IndicadorSituacaoBoleto=2 ;;0- Nenhum, 1- Aberto,
2- Baixado;
DataInicioMovimento=04/03/
DataInicioVencimento=
DataInicioRegistro=
DataFinalMovimento=04/03/
DataFinalVencimento=
DataFinalRegistro=
cnpjCpfPagador=
ContaCaucao=
CodigoEstadoTituloCobranca=
ModalidadeCobranca=
Carteira=
CarteiraVariacao=
IndiceContinuidade=
```
```
02 sResposta String Não
```
```
String com tamanho predefinido para que a mesma possa ser
preenchida com o valor de retorno, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
```
03 esTamanho Integer Não
```
```
Tamanho da string, inteiro que determina o tamanho da string
passada no primeiro parâmetro, mais informações em Como
trabalhar com Strings? (ComotrabalharcomStrings.html)
```
## RETORNO

```
Valor Descrição
```
```
0 Indica que a função foi executada corretamente.
```
```
-10 Indica que houve falhas na execução do método.
```
```
Resposta
```

## [REGISTRO1]

CodRetorno=
ControleCodRetorno=
ControleData=
ControleHora=
ControleNSU=
ControleOriRetorno=
ControleRetorno=
Excecao=
Header_Agencia=
Header_Autenticacao=
Header_CNPJCPF_Beneficiario=
Header_Data_Hora=
Header_Id_Origem=
Header_Id_Processo=
Header_Indice=
Header_Operacao=CONSULTA_BOLETO
Header_Sistema_Origem=
Header_Usuario=
Header_Usuario_Servico=
Header_Versao=
IDCodBarras=
IDLinhaDig=
IDNossoNum=
IDURL=
IndicadorContinuidade=
MsgRetorno=
OriRetorno=
ProximoIndice=

[REGISTRO2]
CodRetorno=
ControleCodRetorno=
ControleData=
ControleHora=
ControleNSU=
ControleOriRetorno=
ControleRetorno=
Excecao=
Header_Agencia=
Header_Autenticacao=
Header_CNPJCPF_Beneficiario=
Header_Data_Hora=
Header_Id_Origem=
Header_Id_Processo=
Header_Indice=
Header_Operacao=CONSULTA_BOLETO
Header_Sistema_Origem=
Header_Usuario=
Header_Usuario_Servico=
Header_Versao=
IDCodBarras=


```
IDLinhaDig=
IDNossoNum=
IDURL=
IndicadorContinuidade=
MsgRetorno=
OriRetorno=
ProximoIndice=
```
```





























