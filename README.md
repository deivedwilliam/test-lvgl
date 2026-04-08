# LVGL XML demo para viewer online

Este workspace contem um mini projeto LVGL XML pensado para demonstracao visual no simulador/viewer online.

Arquivos principais:

- `project.xml`
- `globals.xml`
- `components/metric_card.xml`
- `components/sensor_card.xml`
- `screens/dashboard.xml`
- `screens/report.xml`

O que a interface entrega:

- dashboard elegante para 8 sensores
- cards com leitura, delta e status
- area de operacoes com media, desvio-padrao e diferenca de referencia
- fluxo visual de "gerar relatorio PDF"
- animacao em timeline no refresh e na exportacao

Limite importante:

- no viewer XML puro, a exportacao real de PDF e os calculos dinamicos por selecao precisam de callback/C ou backend
- por isso, este projeto simula a interacao e deixa o layout pronto para ligar a logica real depois

Como usar:

1. Abra a pasta no LVGL Pro Editor.
2. Ou envie os arquivos para um repo e abra no viewer online do LVGL.
3. Teste as telas `dashboard` e `report`.

Se quiser a proxima etapa, da para conectar isso a callbacks em C para:

- recalcular media/desvio em tempo real
- selecionar sensores A/B dinamicamente
- gerar PDF real
"# test-lvgl" 
