# Desafio-de-Projeto---Modelagem-e-Transforma-o-de-dados-com-DAX-com-Power-BI (**Incompleto)
Utilizaremos a tabela única de Financial Sample para criar as tabelas dimensão e fato do nosso modelo baseado em star schema.<br>
O processo consiste na criação das tabelas com base na tabela original. A partir da cópia serão selecionadas as colunas que irão compor a visão da nova tabela. Sendo assim, a partir da tabela principal serão criadas as tabelas:<br>

Financials_origem (modo oculto – backup)<br>

![Descrição do Desafio - Modelagem e Transformação de dados com DAX com Power BI docx (01 02 2025 16_41)](https://github.com/user-attachments/assets/621a6980-e48e-432a-9739-cc2cdeaf55a9)

D_Produtos (ID_produto, Produto, Média de Unidades Vendidas, Médias do valor de vendas, Mediana do valor de vendas, Valor máximo de Venda, Valor mínimo de Venda)<br>

D_Produtos_Detalhes(ID_produtos, Discount Band, Sale Price, Units Sold, Manufactoring Price)<br>

D_Descontos (ID_produto, Discount, Discount Band)<br>

D_Detalhes (*)<br>

D_Calendário – Criada por DAX com calendar()<br>

F_Vendas (SK_ID , ID_Produto, Produto, Units Sold, Sales Price, Discount Band, Segment, Country, Salers, Profit, Date (campos))<br>


*Verifique as informações que não foram contempladas nas demais tabelas dimensão que fornecem maiores detalhes sobre vendas.<br>
