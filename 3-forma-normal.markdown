# Não Normalizada

```
PEDIDO (
    ped_num, cli_cod, cli_nome, cli_endereco, cli_cgc, cli_ie, ite_total_valor,
    ped_total, ven_cod, ven_nome, ped_prazo_entrega (
        prod_cod, pro_unidade, pro_quantidade, pro_descricao, pro_valor_uni
))
```
# 1ª FN

SEPARA GRUPO COM INFORMAÇÕES REPETIDAS.

```
PEDIDO (ped_num, cli_cod, cli_nome, cli_endereco, cli_cgc, cli_ie, ped_total, vem_cod, ven_nome, ped_prazo_entrega)

ITEM-PEDIDO (ped_num, prod_cod, pro_unidade, pro_quantidade, pro_descricao, pro_valor_uni, ite_total_valor)
```

# 2º FN

REMOVE DEPENDÊNCIA FUNCIONAL PARCIAL

```
CLI (cli_cod, cli_nome, cli_endereco, cli_cgc, cli_ie)

PEDIDO (ped_num, ped_total, vem_cod, ped_prazo_entrega, cli_cod)

ITEM-PEDIDO (ped_num, ite_total_valor, prod_cod)

PRODUTO (prod_cod, pro_unidade, pro_quantidade, pro_descricao, pro_valor_uni)
```

# 3º FN

REMOVE DEPENDÊNCIA FUNCIONAL TRANSITIVA

```
VENDEDOR(ven_cod, ven_nome)

PEDIDO (ped_num, ped_total, vem_cod, ped_prazo_entrega, cli_cod)

ITEM-PEDIDO (ped_num, ite_total_valor, prod_cod)

PRODUTO (prod_cod, pro_unidade, pro_quantidade, pro_descricao, pro_valor_uni)
```
