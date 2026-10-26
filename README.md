# Atlas estrutural — Pele de tilápia

Site de consulta acadêmica do galpão com duas linhas: couro de tilápia e PetFish.

## Consulta

- Planta vetorial 2D com pan, zoom, nomes e dimensões de ambientes.
- Modelo 3D com orbitagem, aproximação e cobertura removível.
- 40 ambientes e 76 itens de equipamentos, mobiliário e louças da base R15.
- Pesquisa por sala e equipamento; filtro Couro / PetFish / Apoio.
- Rotas do produto e circulação local ilustrativa de equipes e visitantes.
- Plantas em PDF A0 para consulta e impressão.

## Base e limites

Área coberta nominal de 864 m², terreno hipotético de 3.500 m². A ampliação em relação à ideia inicial de 500 m² corresponde à distribuição da base R15. Áreas são modulares, não levantamento de área útil líquida.

Fonte geométrica: Galpao_Detalhado_A0_R15.dxf e Dados_e_Pontos_R15.json, produzidos no projeto acadêmico. Área externa usa a geometria de referência R13. Equipamentos têm dimensões propostas de implantação, sem fabricante. Formas e alturas 3D são ilustrativas. Paredes rebaixadas permitem consultar o interior.

Linhas de fluxo são esquemáticas. As pessoas representam equipes locais e visitantes, sem comprovação de capacidade ou tempo de ciclo. Não há circulação livre de operadores entre área crua e limpa. A simulação respeita a preferência de movimento reduzido do navegador, com botão para ativar.

Estudo preliminar, não projeto executivo nem comprovação de conformidade normativa. Necessários validação de fluxos, engenharia, acessibilidade, redes, segurança contra incêndio e licenciamento antes da implantação. O site não dimensiona tubulações, cargas elétricas ou tratamento de efluentes.

## Executar localmente

Sirva esta pasta com um servidor HTTP, por exemplo `python -m http.server 8765`, e abra `http://localhost:8765`. Módulos JavaScript não devem ser abertos diretamente por `file://`.

Hospedagem: GitHub Pages, branch `main`, raiz. Sem backend, cadastro, rastreadores ou bibliotecas carregadas por CDN em execução. Three.js 0.170.0 e OrbitControls estão incluídos em `vendor/` sob licença MIT (arquivo `THREE-LICENSE.txt`).

## Arquivos

- `index.html`, `style.css`: interface.
- `app.js`: interações, planta e modelo.
- `data.js`: base de ambientes, equipamentos, paredes e geometria exterior.
- `Planta_A0.pdf`: três pranchas de consulta.

Revisão do site: R16, 26 de outubro de 2026.
