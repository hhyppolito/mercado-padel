# Mercado Padel Portugal

Relatório web sobre empresas ligadas ao padel em Portugal, com informação financeira, comparações e contexto setorial incorporados no HTML.

O título do artefacto atual é «A faturação cresce pouco e os resultados divergem entre empresas de padel». Trata-se de uma publicação analítica, não de uma plataforma de reservas ou marketplace.

## Conteúdo e limites da análise

O ficheiro inclui dados por empresa, indicadores financeiros e referências de fontes. A própria documentação incorporada identifica uma **amostra intencional de 16 NIF**, não um censo de todo o mercado. A cobertura varia entre indicadores e anos.

Comparações devem respeitar o mesmo conjunto de empresas, períodos e definições. Dados de empresas e estatísticas setoriais podem ter universos diferentes; não devem ser somados ou interpretados como equivalentes.

## Estrutura e tecnologia

- [index.html](index.html): relatório, recursos de apresentação e dados incorporados num único ficheiro.
- [README.md](README.md): descrição e orientação de manutenção.

Não existem `package.json`, fontes separadas ou scripts de build na árvore atual. O HTML é um artefacto grande e inclui conteúdo codificado; editar diretamente exige atenção para não corromper recursos.

## Abrir localmente

Com Python 3 instalado:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Abrir [localhost:8000](http://localhost:8000) e consultar as secções e fontes do relatório. Não existe um processo de atualização automática dos dados demonstrado pelos ficheiros deste repositório.

## Atualização e publicação

Preferir regenerar o HTML a partir da fonte de autoria original, caso esteja disponível. Antes de substituir o artefacto:

1. Confirmar origem, data, unidades e cobertura dos dados.
2. Recalcular totais e comparações com a mesma amostra.
3. Atualizar fontes e limitações juntamente com os valores.
4. Testar a apresentação e eventuais controlos do relatório no navegador.
5. Confirmar que os dados incluídos podem ser partilhados no destino escolhido.

O ficheiro pode ser servido por alojamento estático; o estado e configuração da publicação não foram verificados.

## Verificação

A descrição foi baseada no conteúdo HTML inspecionado em 11/11/2026. Esta atualização não recalculou indicadores nem validou as fontes financeiras, e não constitui uma nova análise de mercado. Não foram executados testes de navegador.
