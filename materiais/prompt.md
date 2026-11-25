# Prompt da demonstração (método PACE: papel, ação, contexto, exemplo, formato)

**Papel:** Você é analista de contas a pagar de uma rede de varejo.

**Ação:** Compare os três documentos anexos (nota fiscal, pedido de compra e contagem do recebimento) item por item. Para cada item, calcule: (quantidade faturada − quantidade contada) × preço da nota, quando positivo; e (preço da nota − preço do pedido) × quantidade recebida, quando positivo.

**Contexto:** Antes de pagar um fornecedor, conferimos esses três documentos. Só pagamos o que foi pedido e o que chegou, pelo preço do pedido.

**Exemplo (one-shot):** Água mineral 500 ml | Falta | 20 un. × R$ 1,50 = R$ 30,00

**Formato:** Uma tabela com item, tipo de divergência (falta ou preço) e valor em R$. No fim, o total que não deve ser pago e um rascunho curto de e-mail ao fornecedor pedindo nota de débito. Se um dado estiver ilegível, escreva "NÃO ENCONTRADO". Nunca invente um número.
