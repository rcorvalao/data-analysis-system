# data-analysis-system
Um sistema de análise de dados. O sistema é capaz de importar lotes de arquivos simples, ler e analisar os dados e produzir um relatório.



Layout dos Arquivo simples
 
Existem 3 tipos de dados dentro desses arquivos. Para cada tipo de dados, há um layout diferente.
 
Dados Vendedor
Dados vendedor tem o ID de formato 001 e a linha terá o seguinte formato.
 
001 ç CPF ç Nome ç Salário

Dados do cliente
Os dados do cliente tem o ID de formato 002 e a linha terá o seguinte formato.
 
002 ç CNPJ ç Nome ç Área de Negócios

Os dados de vendas
Dados de vendas tem o ID de formato 003. Dentro da linha de vendas, há a lista de itens, o que é
envolto por colchetes []. A linha terá o seguinte formato.

003 ç Venda ID ç [ID Item - Quantidade Item - Preço Item] ç nome ç nome vendedor



Análise de dados
 
O sistema deve ler dados do diretório padrão, localizado em% HOMEPATH% / data / in.
O sistema só deve ler arquivos .dat.
 
Após o processamento de todos os arquivos dentro do diretório padrão de entrada, o sistema deve criar um arquivo simples
dentro do diretório de saída padrão, localizado em% HOMEPATH% / data / out. O nome do arquivo deve
seguir esse padrão, {} flat_file_name .done.dat.
 
O conteúdo do arquivo de saída deve resumir os seguintes dados:
 
● Quantidade de clientes no arquivo de entrada
● Quantidade de vendedor no arquivo de entrada
● ID da venda mais caro
● Pior vendedor de cada vez
 
Esta aplicação deve estar em execução o tempo todo, sem qualquer quebra. Toda vez que novos arquivos
tornam-se disponíveis, tudo deve ser executado.


