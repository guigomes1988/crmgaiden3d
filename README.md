# Gaiden City · CRM 3D

Protótipo do CRM da **Gaiden Design** em forma de cidade 3D.

| Na cidade | No CRM |
|---|---|
| Prefeitura (centro) | Gaiden Design: orçamento, alíquota padrão e funcionários |
| Empresas nos lotes | Clientes. Cada uma tem segmento, cor da marca e modelo 3D. O tamanho cresce com o fee |
| Aluguel | Fee mensal do cliente |
| Nota fiscal | NFS-e simulada: fee × alíquota = imposto; fee − imposto = líquido |
| Casas no bairro residencial | Funcionários, com o total recebido por mês |
| Prédio em obra (guindaste) | Cliente em negociação |
| Prédio cinza "Fechado" | Cliente cancelado |
| Luz vermelha piscando | Aluguel do mês atrasado |
| Lote disponível | Espaço para um novo cliente |

## Modelos 3D
Prédio comercial, Torre de vidro, Restaurante, Padaria/Café, Loja, Galpão/Logística, Clínica/Saúde, Academia, Escola, Indústria e Hotel.
O segmento escolhido sugere um modelo (ex.: E-commerce → Galpão), mas qualquer modelo pode ser escolhido.

## Regras de cálculo
- **Imposto** = fee × alíquota (padrão global, editável na Prefeitura, ou alíquota própria do cliente).
- **Líquido** = fee − imposto.
- Cada funcionário recebe o **% do líquido** definido no cliente; o que sobra vai para o **caixa da Prefeitura**.
- Só clientes **ativos** entram nos totais. Os em negociação aparecem como "obras".
- **Atraso**: cliente ativo, não marcado como pago no mês e com o dia de vencimento já passado.

## Como usar
Abra o `index.html` em um navegador moderno (precisa de internet para carregar o Three.js do CDN).
Os dados ficam salvos no próprio navegador (localStorage). Use **Exportar/Importar** para fazer backup ou levar para outro computador.

Os clientes de exemplo são fictícios. Edite ou exclua à vontade.
