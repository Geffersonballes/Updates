# Configurando arquivo de documentação das Atualizações do Sistema

## **Página inicial principal da Documentação**


- Para iniciar a formatação da documentação, incluímos primeiramente a logo do **Grupo Scheffer**, que se encontra no caminho ***TI:\logos\Logo documentação\logo.JPG***.
- Seguido do nome do setor com uma cerquilha **(#)** para identificá-lo como título principal.
- Depois acrescentamos três hifens **(---)** para fazer um linha de réguia horizontal.
- Dentro do bloco colocamos as informações padrão com as seguintes configurações do exemplo:
```  
SISTEMA: **ERP – Sapiens**    
MÓDULO: **Setor onde está sendo feito o tesde da atualização**    
VERSÃO ATUAL: **Versão atual do sistema**     
VERSÃO TESTE: **Versão que está sendo testada**     
RESPONSÁVEL: **Nome do responsável pelo teste da nova aturalização**    
CRIADO EM: **Data da criação da documentação**" 

```
- Em seguida, acrescentamos mais uma linha de régua com **(---)**.
- Por padrão são essas as configurações de formatação inicial da documentação de atualização.
- Para configurar os indices de ***Entendimentos*** configuramos com os seguintes parâmetros.

```
### Entendimentos  
#### Introdução (nas citações da versão atual e a versão de teste é feito em negrito, com dois asteriscos (**))  
#### Objetivo  
#### Conclusão  
#### Exclusões específicas  
#### Atividades e Estratégias de Homologação  
#### Fatores de Sucesso da Homologação

```
## **Títulos Principais**

### Telas onde são feito os testes da versão

- Os títulos principais (Telas onde é feito os testes da versão) são configurados com dois ***##*** e em negrito **(```**```)**, exemplo:

```
## **F420GOC_SCOC - Suprimentos / Gestão de Compras / Ordens de Compra / Agrupada**

```

### **Notas das Versões**

- Inicialmente colocamos o título ***"Notas da Versão 5.8.9.18"*** com três cerquilhas **(###)**, e criamos um bloco para colocarmos as notas da versão que está sendo testada. Para isso usamos a extensão ***!!! note ** *** e, na linha de baixo colocamos o título da versão em negrito. Exemplo:

``` 
### Notas da Versão 5.8.9.18

!!! note ""  
	**Erro no processamento da ordem de compra**  

```

- Nas ***Notas da Versão*** tem os tópicos ***Problema*** e ***Correção efetuada***. Colocar as palavras ***Problema*** e ***Correção efetuada*** em negrito.
- Todas as citações de telas, regras, registros, títulos, mensagens de erros do sistema, e itens que há nas notas da versão tem que ser digitado em negrito.
- Todas as citações de botão, campo, tags, idiomas e outras citações de parâmetros menos importantes da versão deve estar em sublinhado. Exemplo:

```
### Notas da Versão 5.8.8.68

!!! note ""
	**Mensagem de erro na validação do *SPED Contribuições***  

	**Problema:** na validação do *SPED Contribuições* ocorria a seguinte mensagem no 
    registro *C181:* **Valor informado deve ser maior que zero campo Valor Total do 
    Item.** O problema ocorria, pois uma nota fiscal de complemento de ICMS, NF de 
    saída tipo 9, era listada no *SPED Contribuições*, e nessa nota fiscal só existia o 
    valor do ICMS preenchido.  

	**Correção efetuada:** ajustamos a geração de nota fiscal de saída do tipo *Acerto*
    para que não obrigue ao usuário informar as *CST de ICMS, IPI, PIS e COFINS* quando
    for executada a regra **522**.  
    Ajustamos também, a geração de nota fiscal de entrada do tipo *Acerto/complemento* 
    para que não obrigue ao usuário informar as *CST de ICMS, IPI, PIS e COFINS* quando 
    for executada a regra **514**. Alteramos as regras **519** e **559** para não 
    obrigarem a situação tributária de ICMS das notas de Acerto.
    
```
## **Tabelas de *Testes***

- As tabelas de testes é feito conforme está no arquivo original da Documentação. Com o título com duas serquilhas **( ### )**. Separando apenas as colunas e linhas. Exemplo:

```
### Teste

Campo da Tela | Valor  
 - | - 
N° DA ORDEM DE COMPRA | 33.679  
EMISSAO DA OC. | AUTOMOTIVO 14/03/2017
TRANSAÇÃO DO PRODUTO |	90410 
FORNECEDOR | 	668
PEDIDO FORNECEDOR |	123
MOEDA |	03
SAFRA |	2016/2017
OBS: |	COMPRA DE DEFENSIVO PARA FAZ. RAFAELA 

```

### Teste

Campo da Tela | Valor  
 - | - 
N° DA ORDEM DE COMPRA | 33.679
EMISSAO DA OC. | AUTOMOTIVO 14/03/2017
TRANSAÇÃO DO PRODUTO |	90410 
FORNECEDOR | 	668
PEDIDO FORNECEDOR |	123
MOEDA |	03
SAFRA |	2016/2017
OBS: |	COMPRA DE DEFENSIVO PARA FAZ. RAFAELA 

- Seguido das imagens das telas de testes do sistema.