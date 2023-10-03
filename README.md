# CASE-MARKETING-

# Estudo do Perfil dos Clientes

# Briefing

Com a finalidade de entender melhor o perfil dos clientes para potencializar a venda de um produto de investimento, a área de marketing criou uma campanha selecionando alguns clientes para realizar a oferta. A duração da campanha foi de 3 meses e abrangeu todo o Brasil.

Finalizada a campanha, o marketing disponibilizou a base de dados (bank_marketing.xlsx) e solicitou uma análise do perfil dos clientes à área de Analytics. A expectativa é que esse estudo forneça informações suficientes para que as próximas campanhas sejam direcionadas para o público mais propenso a comprar o produto do investimento.

Sua missão, como Analista de Dados, é responder a seguinte pergunta de negócios: Qual é o perfil dos nossos clientes? Para responder de forma adequada, você deve:

 - Realizar uma Análise Exploratória buscando por insights sobre a venda dos títulos, o perfil dos clientes: Idade, Profissão, Estado Civil, Formação,    Situação de Crédito e sobre a utilização de outros produtos: Hipoteca e Empréstimo.

 - Construir um relatório que embase com dados os insights encontrados, e traduza termos mais técnicos para a linguagem de negócios.



# Resolução 

# 1. Importar e revisar o conjunto de dados

Importar o dataset no Excel.

![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/03c98f4a-ab2d-4473-8436-6d1cb33f5970)

O conjunto de dados possui 9684 linhas, sendo que cada linha representa um cliente único.

As colunas que armazena são:

- Cliente_Comprou_o_Título?: Retorna com "Sim", caso o cliente tenha comprado o título e "Não", caso não tenha comprado.
- Idade: Idade do cliente.
- Profissão: Ocupação profissional do cliente. 
- Estado Civil: Retorna uma das três opções: "Solteiro", "Casado" ou "Divorciado".
- Formação: Retorna a escolaridade do cliente: "Fundamental", "Ensino Médio" ou "Ensino Superior".
- Cliente_Devedor?: "Sim" ou "Não" se o cliente é devedor ou não. 
- Saldo_Conta_Corrente: Valor em reais do saldo da conta corrente do cliente.
- Tem_Hipoteca?: "Sim" ou "Não" se o cliente tem hipoteca ou não. 
- Tem_Empréstimo?: "Sim" ou "Não" se o cliente tem algum tipo de empréstimo ou não. 
- Qte_de_Ligações_Feitas: Mostra a quantidade de ligações efetuadas para cada cliente.


# Análise Exploratória dos Dados

# Resumir o total de clientes que comprou o produto e a porcentagem

# Insights
- Quase metade dos clientes compraram o produto.
- (Perguntar ao especialista do negócio qual é o referencial histórico da % de compra)

  

![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/b326940f-cb0c-4d28-8f96-ea455e43fb4b)



![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/ecfcdb49-8bdb-456e-8418-ed5b6d97b8e3)

Criar um gráfico de rosca (duas alternativas possibilitam o uso desse tipo de gráfico) para visualizar a informação: 


# Resumir a faixa etária do total dos clientes, com acréscimo da porcentagem dos clientes acumulada 

# Insights

- A faixa Etária com maior número de clientes é a de 28 a 37 anos.
- Quase 90% dos clientes têm até 57 anos de idade.

  
  
![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/e4db799b-79c1-49fe-bd6f-d547418440f0)

![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/4280e728-9e71-41dc-b986-f56b13c06833)

Gráfico de pareto usado para adicionar a % acumulada no eixo secundário.


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/d585b3f4-53ca-424b-9c03-c88050ff0edf)

Gráfico boxplot para identificar os quartis, média, mediana e outliers.


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/2d1fa7bd-ec05-4d0b-9afe-c0a4d60308e4)

Gráfico de histograma para identificar a onda de variação.



# Total de clientes e suas respectivas profissões 

# Insights

- A profissão Administrador é a mais frequente entre os clientes (35%).
- As profissões mais frequentes são Administrador (35%), Operário (17%), Técnico (16%) e Serviços Gerais (8%). Juntas, correspondem a 76% dos clientes.
  


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/65cf5a0f-4921-4aac-ada5-b6679e8ddfc1)

("Desconhecido" destacado para auxiliar nas atualizações da tabela base) 


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/dea8c7b1-4b7c-4a7d-add1-338d7f28fac8)


Gráfico de pareto para identificar o % por acúmulo de profissões.




# Total de clientes de acordo com o Estado Civil 

# Insights

- Mais da metade (57%) dos clientes são casados.
- Existe a informação do número de filhos/dependentes?

  

![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/2b58b4c3-da1a-4d0c-a3da-92acc9ee9407)

![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/a5dad14b-2578-4979-9f0e-bdb3035e01e1)





# Total de clientes de acordo com a formação

# Insights

- Quase metade dos clientes possuem Ensino Médio (49%).
- Cerca de 62% dos clientes possuem até o Ensino Médio.


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/3aff77b6-8dce-458e-a67f-93aeca515e95)


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/df53e183-b922-485b-bb06-6e21abda73fc)



# Total de clientes devedores

# Insights

- 99% dos clientes não são devedores.
- (Perguntar ao especialista como foi realizada a seleção dos clientes para a campanha)



![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/0747a28d-4a46-4feb-81cd-99418f75ce52)


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/901bfb3d-f0ad-4ad1-9af8-d5a3e4cdc079)




# Total de clientes e os valores em conta corrente de cada cliente 

# Insights

- 84% dos clientes possuem até R$ 3.000,00 de saldo em conta corrente.
- Apenas 2% dos clientes possuem mais de R$ 10.000,00 em conta corrente.
- Grande parte dos clientes possuem baixo valor de saldo em conta corrente, enquanto poucos clientes possuem um saldo mais alto em conta corrente.



![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/4ee70f7b-c51f-47aa-8f5d-9983d376c8a7)


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/7a5d6682-5903-4091-9c1d-ac274ca4d4ad)



![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/e0dd5bb4-7117-403d-b91c-f3832110e209)



![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/6639d0b0-68ad-4b51-9092-ffcdb7e62407)





# Total de clientes que possuem hipoteca 

# Insights

- A maioria dos clientes (54%) não possuem hipoteca.
- Qual a comparação entre os juros pagos pela hipoteca e os juros do rendimento da aplicação no título de investimento?
  


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/27860265-eeec-4dc9-b708-2555c232915b)


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/959b762e-8676-4b06-a518-d3659f3e0954)




# Total de clientes que possuem empréstimo 

# Insights

- A grande maioria dos clientes (88%) não possuem empréstimo.
- O cliente possuir empréstimo dificulta a aquisição de um título de investimento?


![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/a0980ef0-5b40-4dda-916f-2ba2a4fa6317)

![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/505d9cb2-f053-40fc-8c72-7ba2f91346c3)




# Quantidade de ligações por cliente 

# Insights

- Em aproximadamente 82% dos clientes foi necessário realizar entre 1 e 3 ligações para fazer a apresentação e obter uma resposta sobre a compra do título.
- 95% dos clientes foram contatados em no máximo 6 ligações.

  

![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/a9038709-68da-42e5-a230-97715a08a72a)

![image](https://github.com/abneroliveiraa/CASE-Preditiva-Analytics/assets/146268340/fdb00bbc-9713-44ca-a1d7-70f1bf0e4510)

