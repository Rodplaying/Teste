# Simulador de Vendas · Painéis Solares

Simulador comercial configurável para propostas de sistemas fotovoltaicos. É um único ficheiro HTML: basta abrir `index.html` num browser.

## Simulação
- Dados do cliente: região, perfil de consumo, consumo mensal (kWh ou fatura em €), preço da eletricidade, cobertura alvo, modelo e nº de painéis, desconto.
- Opções: bateria, financiamento e apoio estatal.
- Resultados: potência (kWp), investimento ou prestação mensal, poupança no 1.º ano, retorno do investimento, ROI, autossuficiência, CO₂ evitado, gráficos e projeção ano a ano.
- Rentabilidade interna da venda (custos, comissão, lucro, €/Wp), escondida na proposta impressa.
- Botão "Proposta (PDF)" para imprimir/guardar a proposta para o cliente.

## Histórico e backup
- "Guardar simulação" guarda o cliente (nome, contacto, notas), os dados introduzidos e os resultados no histórico deste aparelho.
- No separador Histórico: procurar, abrir (recalcula com os preços atuais), editar e apagar simulações.
- "Enviar backup" abre a partilha do telemóvel com um ficheiro de backup (.txt) e uma folha CSV para o Excel; no computador, descarrega os dois ficheiros.
- "Restaurar backup" junta as simulações de um backup sem duplicar e, opcionalmente, repõe a configuração.

## App instalável (PWA)
- Publicada no GitHub Pages pelo workflow `.github/workflows/pages.yml` a cada push.
- No Android: abrir o endereço no Chrome e escolher "Instalar app" (ou menu ⋮ > Adicionar ao ecrã principal). Funciona sem internet.

## Configuração
- Catálogo de painéis, regiões (produção kWh/kWp/ano) e perfis de cliente, todos editáveis.
- Custos (inversor, estrutura, mão de obra, fixos, bateria), margem, IVA, comissão, desconto máximo, preço do excedente, inflação da energia, manutenção, apoios, juro e prazo de financiamento, limites do semáforo de retorno.
- Guardada automaticamente no browser (localStorage); exportar/importar em JSON e repor valores de fábrica.

Os valores por defeito são estimativas indicativas para Portugal e devem ser ajustados à realidade da empresa.
