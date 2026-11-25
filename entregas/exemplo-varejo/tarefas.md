# Mapa de tarefas — exemplo (pagamento a fornecedores de uma rede de varejo)

**Problema:** a empresa paga fornecedores por mercadoria que não chegou ou com preço acima do pedido.

**Processo:** conferir e pagar cerca de 10 mil notas fiscais de fornecedores por mês. Números adaptados de um caso real.

| Tarefa | Quem é pago para fazer hoje? | Custo hoje (por unidade × vezes por mês) | Custo de um erro | Decisão (regra, IA ou humano) | Justificativa |
|---|---|---|---|---|---|
| 1. Capturar a nota fiscal | Ninguém: o sistema fiscal já faz | Quase zero × 10 mil | Baixo | Regra | Já resolvido por software; não há negócio de IA aqui. |
| 2. Conferir nota × pedido × contagem do recebimento | Analistas, em 99% das notas | Parte dos ~R$ 4 por nota × 10 mil | Alto: em média ~R$ 47 por nota pagos a mais | IA confere; humano só nas divergências | Volume alto e erro caro: a IA confere tudo, a pessoa decide as exceções. |
| 3. Programar o pagamento até o vencimento | Analistas e tesouraria | Parte dos ~R$ 4 por nota × 10 mil | Alto: juros e fornecedor bloqueando entregas | Regra | Depois da conferência, uma fila pela data de vencimento resolve. |
| 4. Cobrar do fornecedor o que foi pago a mais | Praticamente ninguém | Hoje não é feito | Médio | IA redige; humano envia | Dinheiro parado na mesa; a IA prepara a cobrança com a evidência. |
| 5. Negociar com fornecedor que bloqueou entregas | Comprador | Poucas vezes por mês | Alto | Humano (copiloto prepara) | Volume baixo e erro caro: relação comercial não se automatiza. |

**Tarefa escolhida para a entrega de automação:** 2. Conferir nota × pedido × contagem do recebimento.
