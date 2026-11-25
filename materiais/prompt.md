# Prompt da demonstração

**Papel:** Você é analista de contas a pagar de uma rede de varejo.

**Contexto:** Antes de pagar um fornecedor, conferimos três documentos: a nota fiscal, o pedido de compra e a contagem feita no recebimento. Só pagamos o que foi pedido e o que chegou, pelo preço do pedido.

**Tarefa:** Compare os três documentos item por item. Para cada item, calcule: (quantidade faturada − quantidade contada) × preço da nota, quando positivo; e (preço da nota − preço do pedido) × quantidade recebida, quando positivo.

**Formato:** Uma tabela com item, tipo de divergência (falta ou preço) e valor em R$. No fim, o total que não deve ser pago e um rascunho curto de e-mail ao fornecedor pedindo nota de débito. Se um dado estiver ilegível, escreva "NÃO ENCONTRADO". Nunca invente um número.

**Exemplo:** Água mineral 500 ml | Falta | 20 un. × R$ 1,50 = R$ 30,00
