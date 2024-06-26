# ENTIDADES
### PRODUCT
* ID - UUID
* SIZE - NUMBER (CM)
* COLOR - STRING
* POPULAR - BOOLEAN
* CREATED_AT - DATE
* VALUE - NUMBER
* DEPOSIT_ID - UUID - DEPOSIT

* PURCHASE_ORDERS []
--------------------------------------------------
### DEPOSIT
* ID - UUID
* PRODUCT_ID - UUID - PRODUCT
* AMOUNT - NUMBER
* MINIMUM_LIMIT - NUMBER
* CREATED_AT - DATE
--------------------------------------------------
### SALE
* ID - UUID
* CREATED_AT - DATE

* PRODUCT_SOLD []
--------------------------------------------------
### PRODUCT_SOLD
* ID - UUID
* SALE_ID - UUID - SALE
* PRODUCT_ID - UUID - PRODUCT_ID
* AMOUNT - NUMBER
* VALUE - NUMBER
* CREATED_AT - DATE
--------------------------------------------------
### PURCHASE_ORDERS
* ID - UUID
* PRODUCT_ID - UUID - PRODUCT_ID
* AMOUNT_PRODUCT - NUMBER
* VALUE - NUMBER
* EXPENSES - NUMBER
* CREATED_AT - DATE
* RECEIVED_AT - DATE | NULL
--------------------------------------------------
# CASOS DE USO
* Visualizar um ou varios produto
* Cadastrar um produto
* Atualizar um produto
* Excluir um produto
* Visualizar uma ou varias vendas
* Realizar uma venda
* Visualizar o estoque
* Receber um aviso via e-mail ou receber no propria aplicação, quando a quantidade minima de qualquer produto ser atingida
* Criar ordens de compra automaticamente
* Gerenciar ordens de compra
* Receber atualizações dos fornecedores sobre os prazos de entrega de novas remessas
  
