
▓▓▓▓▓▓ Colunas / Medidas ▓▓▓▓▓▓

-> Coluna Calculada
Cria uma coluna e calcula linha a linha


-> Medidas implícitas
É criada pelo próprio Power bi 

-> Medidas Explícitas

-> Variáveis 

-> Iteradores 


▓▓▓▓▓▓ Funções e Formulas  ▓▓▓▓▓▓


Conta os dias entre datas:
-> LeadTime = INT('nome da tabela'[Data_Entrega] - 'nome da tabela'[Data_Compra])


Funções

INT 	-> Transforma em numero inteiro
SUM 	-> Soma os valores
AVERAGE  -> Essa função tira a media 
	->


░░░░░░  5Tecnicas de redução de arquivos ░░░░░░

	Remoção e Redução  	
		Colunas
		► Toda coluna importa (sempre use a quantidade de colunas necessário)
		► Adicionar x Remover colunas (filtragem vertical)

 		Linhas 
		► Menor nº possível (Filtragem horizontal) 
		► Tempo, entidade, característica 
		► Delimitar os dados só para o necessário

	Agrupar por e Resumir
		► Alto eficiência na redução do tamanho de um modelo.
		► Redução de granularidade do conjunto de dados.
		Exemplo: agrupar um coluna de data (perder os detalhes), mas ganho no desempenho.  

	Otimizar tipos de dados
		► Auxilio no mecanismo de armazenamento
			-> value encoding = dados numéricos
			Exemplo: https://medium.com/aiskunks/categorical-data-encoding-techniques-d6296697a40f
			-> dictionary encoding = string (de-para)
			Exemplo:https://medium.com/aiskunks/categorical-data-encoding-techniques-d6296697a40f
			-> run length encoding = reduzir repetições de valores

		► Identificadores na estrutura de dados para a pesquisa de hash durante o armazenamento e consulta.
			Divisão das colunas e real necessidade de ambas.
	
	Preferência por colunas personalizadas
		► Envolve bom conhecimento nos processos de criação de colunas calculadas.
		►  Colunas computadas pelo POWER QUERY (linguagem M) x Colunas Dax.

	Desabilitar Data e Hora Automática
		► Importância de uma tabela calendário em grande conjunto de dados.
		► Geração de hierarquia automática em todas as tabelas que contém campos de data/hora (usar tabela calendário)
	
			
  
https://learn.microsoft.com/pt-br/power-bi/guidance/import-modeling-data-reduction?source=docs


----------- Desafios -------------

Media do Leadtime com iterado = AVERAGEX('buscante_registro_vendas', INT('buscante_registro_vendas'[Data_Entrega] - 'buscante_registro_vendas'[Data_Compra]) )

- Quantidade máxima de produtos 
- Somatório dos preços
- Total de descontos

- Total de produtos
- Margem bruta por porcentagem
- Soma da margem bruta 
- Soma do custo total



Estimativa de ganhos

Soma  (Quant. de produtos * Quant. preço unitário )
X + (A * B)


custo bruto = Preço de custo * Quantidade de vendas
faturamento total = Preço Unitário * Quantidade de vendas
margem bruta  =  faturamento total - custo bruto
margem bruta por %  = margem bruta / faturamento total


  



 








