# 🛰️ TerraLens AI v4.0
### Plataforma de Inteligência Artificial Geoespacial e Análise 360°

[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel)](https://terralens-ai.vercel.app)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/Version-4.0-blue?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-Beta-orange?style=for-the-badge)]()
[![ML/DL](https://img.shields.io/badge/ML%2FDL-40%2B%20Modelos-purple?style=for-the-badge)]()
[![CV](https://img.shields.io/badge/Computer%20Vision-Bounding%20Boxes-cyan?style=for-the-badge)]()

> **🚀 Acesse agora:** [terralens-ai.vercel.app](https://terralens-ai.vercel.app)
> 
> **💻 Código aberto:** [github.com/flaviocaos/terralens-ai](https://github.com/flaviocaos/terralens-ai)

---

## 📌 Sobre o Projeto

O **TerraLens AI** é uma plataforma profissional de **Inteligência Artificial aplicada à análise geoespacial** que roda **100% no navegador**, sem instalação, sem cadastro e sem backend. Combina **Machine Learning**, **Deep Learning** e **Computer Vision** para gerar relatórios técnicos completos a partir de imagens de satélite, drone e imagens 360°.

---

## 🤖 A IA por trás da plataforma

| Tecnologia | Modelos | Aplicação |
|------------|---------|-----------|
| **Machine Learning** | Random Forest, XGBoost, SVM | Classificação LULC, vigor, erosão, solos |
| **Deep Learning** | U-Net, DeepLab v3+, SegFormer, YOLOv8, RT-DETR, Mask R-CNN | Segmentação semântica, detecção de objetos |
| **Computer Vision** | K-Means clustering, proxies espectrais RGB, análise de textura e entropia | Processamento 100% no browser |
| **LPR/ALPR** | LPRNet, WPOD-NET, TrOCR | Reconhecimento de placas veiculares |
| **Crack Detection** | CrackFormer, U-Net Crack | Patologias estruturais |
| **Transformers** | ViT, CLIP, SegFormer-B4, RT-DETR | SOTA para detecção e classificação |

---

## ✨ Funcionalidades

### 🛰️ Satélite / Drone / Google Earth — 21 análises com IA

| Categoria | Análise | Modelos Recomendados |
|-----------|---------|---------------------|
| 🌍 Cobertura | Classificação LULC | Random Forest, U-Net |
| 🌿 Vegetação | Vigor e Biomassa, Cobertura Florestal, Desmatamento | RF Regressor, EfficientNet |
| 🏙️ Urbano | Expansão Urbana, Extração de Telhados | SegFormer-B2, YOLOv8-seg |
| 💧 Hidrologia | Dinâmica Hídrica, Inundação | NDWI+MNDWI, U-Net Hydro |
| 🚰 Infraestrutura | Saneamento e Esgoto | RF Sanitário, NDTI |
| 🌾 Agro | Agricultura de Precisão, Solos | RF Zonas, XGBoost |
| 🗺️ Cartografia | Vetorização Automática, Extração de Vias | D-LinkNet, SAM |
| ☀️ Energia | Potencial Solar Fotovoltaico | RF Solar, CNN Solar |
| 🌡️ Ambiental | Carbono, Queimadas, Erosão, Mineração | NBR+dNBR, CNN Alert |
| ⛰️ Topografia | Análise Topográfica | DEM Analysis, TPI+TRI |
| 📈 Espectral | Índices NDVI, GLI, VARI, EVI | Stack RGB JS |
| 🏠 Imobiliário | Avaliação de Terrenos | RF Avaliador, OBIA |

### 🔄 Imagens 360° — 14 análises urbanas com Computer Vision

| Categoria | Análise | Detecção |
|-----------|---------|----------|
| 🛣️ Pavimento | Buracos e Trincas | Bounding box por contraste |
| 💡 Elétrico | Postes e Fiação | Detecção por cor e posição |
| 🚦 Sinalização | Placas de Trânsito | Detecção por proxy vermelho |
| 🚗 Veículos | Placas LPR, Contagem | Detecção por cor amarelo/cinza |
| 🏢 Estrutural | Fachadas, Rachaduras, Inspeção | Análise de brilho e contraste |
| 🌳 Verde Urbano | Arborização | GLI + proxy verde RGB |
| ♿ Urbano | Acessibilidade, Comércios | Análise espectral por grid |
| 🗑️ Ambiental | Lixo Irregular | Detecção por anomalia espectral |
| 🚶 Pessoas | Pedestres e Fluxo | Análise de densidade cromática |

---

## 🎯 Detecção 360° com Bounding Boxes

Funcionalidade exclusiva para imagens 360°:

- ✅ **Corte automático** — remove céu (22% topo) e capô (28% fundo), preservando a faixa útil
- ✅ **Bounding boxes** desenhados via Canvas API com cantos decorativos
- ✅ **Labels com confiança** — ex: `Vegetacao 87%`, `Veiculo 95%`, `Fachada 82%`
- ✅ **Detector específico por análise** — cada uma das 14 análises tem critérios próprios de cor, brilho e posição
- ✅ **Merge de células adjacentes** — agrupa detecções próximas em um box único
- ✅ **Comparativo** Original vs Detecção lado a lado

---

## 📊 Relatório Técnico Completo

Cada análise gera relatório com 4 abas:

- 📋 **Visão Geral** — KPIs, gauges animados, donut chart de cobertura
- 📊 **Gráficos** — Radar chart 6D, histograma NDVI, histograma RGB por canal, métricas de textura
- 🗺️ **Mapas** — Original, LULC K-Means, NDVI RdYlGn, Falsa Cor BGR
- 📄 **Relatório** — Interpretação técnica, perfil da imagem, alertas, recomendações, metodologia

Para imagens 360°, aba adicional:
- 🎯 **Detecção 360°** — imagem cortada + bounding boxes + lista de detecções com confiança

---

## ⚡ Tecnologias

```
Frontend:      React 18 + JSX (Babel CDN)
Processamento: Canvas API + JavaScript puro (zero dependências)
Algoritmos:    K-Means clustering, proxies espectrais RGB
               Análise de textura, entropia, contraste
Detecção 360°: Grid espectral + bounding boxes via Canvas
Mapas:         LULC K-Means, NDVI RdYlGn, Falsa Cor BGR
Gráficos:      SVG puro (Gauge, Radar, Donut, Histograma RGB)
Deploy:        Vercel (CDN global, deploy automático)
Repositório:   GitHub (integração automática com Vercel)
```

---

## 🚀 Como usar

1. Acesse [terralens-ai.vercel.app](https://terralens-ai.vercel.app)
2. Escolha o modo: **🛰️ Satélite/Drone** ou **🔄 Imagens 360°**
3. Filtre por categoria (Urbano, Ambiental, Agro, etc.)
4. Faça upload da imagem (PNG, JPG, TIFF, WebP)
5. Selecione o tipo de análise
6. Escolha o modelo ML/DL na ficha técnica
7. Clique em **Gerar Relatório**
8. Explore as abas: Visão Geral, Gráficos, Mapas, Relatório
9. Para 360°: explore a aba **Detecção 360°** com bounding boxes

---

## 🖥️ Rodar localmente

```bash
git clone https://github.com/flaviocaos/terralens-ai.git
cd terralens-ai
# Abra o index.html no navegador — zero instalação!
```

---

## ⚠️ Status — Versão Beta

Esta é uma versão **Beta** em fase de testes com a comunidade.

**Limitações atuais:**
- Índices espectrais calculados via proxies RGB (sem NIR real)
- Classificação K-Means não supervisionada
- Detecção 360° usa análise espectral por grid — para produção real os modelos precisam de treinamento supervisionado com datasets específicos
- Modelos ML/DL listados são referência técnica para implementação em ambiente Python/GPU
- Claude Vision disponível apenas com API key configurada

**Próximas versões planejadas:**
- [ ] Integração com Claude Vision API ativa
- [ ] Modelos YOLOv8 treinados com datasets específicos
- [ ] Suporte a imagens multiespectrais reais (Sentinel-2, Landsat)
- [ ] Export de relatório em PDF
- [ ] Georreferenciamento das detecções com GPS
- [ ] Histórico e comparação temporal de análises
- [ ] App mobile (PWA)

---

## 📬 Contato e Feedback

- 🐛 [Abrir uma Issue](https://github.com/flaviocaos/terralens-ai/issues)
- 💼 [LinkedIn](https://linkedin.com/in/flaviocaos)
- ⭐ Se gostou, deixe uma estrela no repositório!

---

## 📄 Licença

[MIT License](LICENSE) — use, modifique e distribua livremente.

---

<div align="center">

**Feito com ❤️ + IA + ML + DL**

🛰️ **TerraLens AI v4.0** · 35 análises · ML/DL/CV · 100% Front-End · Vercel

</div>
### Plataforma de Inteligência Geoespacial e Análise 360° com IA

[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel)](https://terralens-ai.vercel.app)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/Version-4.0-blue?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-Beta-orange?style=for-the-badge)]()

> **🚀 Acesse agora:** [terralens-ai.vercel.app](https://terralens-ai.vercel.app)

---

## 📌 Sobre o Projeto

O **TerraLens AI** é uma plataforma profissional de análise geoespacial que roda **100% no navegador**, sem instalação, sem cadastro e sem backend. Combina algoritmos de Machine Learning, Deep Learning e processamento de imagens para gerar relatórios técnicos completos a partir de imagens de satélite, drone e imagens 360°.

---

## ✨ Funcionalidades

### 🛰️ Análises de Satélite / Drone / Google Earth — 21 análises

| Categoria | Análises |
|-----------|----------|
| 🌍 Cobertura | Classificação LULC |
| 🌿 Vegetação | Vigor e Biomassa, Cobertura Florestal, Alerta de Desmatamento |
| 🏙️ Urbano | Expansão Urbana, Extração de Telhados |
| 💧 Hidrologia | Dinâmica Hídrica, Mapeamento de Inundação |
| 🚰 Infraestrutura | Saneamento e Esgoto |
| 🌾 Agro | Agricultura de Precisão, Classificação de Solos |
| 🗺️ Cartografia | Vetorização Automática, Extração de Vias |
| ☀️ Energia | Potencial Solar Fotovoltaico |
| 🌡️ Ambiental | Estoque de Carbono, Queimadas, Erosão, Mineração |
| ⛰️ Topografia | Análise Topográfica |
| 📈 Espectral | Índices Espectrais (NDVI, GLI, VARI) |

### 🔄 Análises de Imagens 360° — 14 análises

| Categoria | Análises |
|-----------|----------|
| 🛣️ Pavimento | Reconhecimento de Buracos e Trincas |
| 💡 Elétrico | Inventário de Postes e Luminárias |
| 🚦 Sinalização | Placas de Rua e Sinalização de Trânsito |
| 🚗 Veículos | Placas de Automóveis (LPR/ALPR), Detecção de Veículos |
| 🏢 Estrutural | Análise de Fachadas, Rachaduras e Patologias, Inspeção Predial |
| 🌳 Verde Urbano | Inventário de Arborização |
| ♿ Urbano | Acessibilidade Urbana, Mapeamento de Comércios |
| 🗑️ Ambiental | Descarte Irregular de Lixo |
| 🚶 Pessoas | Detecção e Contagem de Pedestres |
| 🔵 Drenagem | Reconhecimento de Bueiros |

---

## 📊 Relatório Técnico Completo

Cada análise gera um relatório com:

- 📋 **Visão Geral** — KPIs, gauges animados, donut chart
- 📊 **Gráficos** — Radar chart, histograma NDVI, histograma RGB por canal, métricas de textura
- 🗺️ **4 Mapas Temáticos** — Original, LULC K-Means, NDVI Proxy RdYlGn, Falsa Cor BGR
- 🖼️ **Perfil da Imagem** — Resolução, brilho, contraste, entropia, qualidade espectral
- 📄 **Relatório PDF-ready** — Interpretação técnica, alertas, recomendações, metodologia

---

## 🤖 Modelos ML/DL disponíveis

Cada análise oferece **4 opções de modelos** com ficha técnica completa:

- ✅ Complexidade (Baixa/Média/Alta)
- ✅ Necessidade de GPU
- ✅ Tempo estimado de processamento
- ✅ Acurácia esperada
- ✅ Prós e contras

**Modelos disponíveis:** Random Forest, XGBoost, U-Net, DeepLab v3+, YOLOv8, SegFormer, Mask R-CNN, RT-DETR, EfficientNet, SAM, D-LinkNet, CrackFormer, LPRNet, ViT, CLIP e mais.

---

## ⚡ Tecnologias

```
Frontend:     React 18 + JSX (via Babel CDN)
Processamento: Canvas API + JavaScript puro
Algoritmos:   K-Means clustering, proxies espectrais RGB
Mapas:        LULC, NDVI RdYlGn, Falsa Cor BGR
Gráficos:     SVG puro (Gauge, Radar, Donut, Histograma)
Deploy:       Vercel (CDN global)
Repositório:  GitHub
```

---

## 🚀 Como usar

1. Acesse [terralens-ai.vercel.app](https://terralens-ai.vercel.app)
2. Escolha o modo: **🛰️ Satélite/Drone** ou **🔄 Imagens 360°**
3. Faça upload da imagem (PNG, JPG, TIFF, WebP)
4. Selecione o tipo de análise
5. Escolha o modelo ML/DL
6. Clique em **Gerar Relatório**
7. Explore as 4 abas: Visão Geral, Gráficos, Mapas e Relatório

---

## 🖥️ Rodar localmente

Não precisa de instalação! Basta abrir o arquivo `index.html` em qualquer navegador moderno:

```bash
git clone https://github.com/flaviocaos/terralens-ai.git
cd terralens-ai
# Abra o index.html no navegador
```

---

## ⚠️ Status — Versão Beta

Esta é uma versão **Beta** em fase de testes com a comunidade.

**Limitações atuais:**
- Índices espectrais calculados via proxies RGB (sem NIR real)
- Classificação K-Means não supervisionada
- Modelos ML/DL listados para referência técnica (execução requer ambiente Python)
- Claude Vision disponível apenas em deploy com API key configurada

**Próximas versões:**
- [ ] Integração com Claude Vision API
- [ ] Suporte a imagens multiespectrais reais
- [ ] Export de relatório em PDF
- [ ] Histórico de análises
- [ ] Comparação temporal de imagens

---

## 📬 Contato e Feedback

Encontrou um bug? Tem sugestão? Quer contribuir?

- 🐛 [Abrir uma Issue](https://github.com/flaviocaos/terralens-ai/issues)
- 💼 [LinkedIn](https://linkedin.com/in/flaviocaos)
- ⭐ Se gostou, deixe uma estrela no repositório!

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE) — sinta-se livre para usar, modificar e distribuir.

---

<div align="center">

**Feito com ❤️ e IA**

🛰️ **TerraLens AI v4.0** · 35 análises · 100% Front-End · Vercel

</div>

## 🤝 Como Contribuir

1. Faça um **Fork** do repositório
2. Crie uma branch: `git checkout -b feature/MinhaFeature`
3. Commit suas mudanças: `git commit -m 'Add MinhaFeature'`
4. Push para a branch: `git push origin feature/MinhaFeature`
5. Abra um **Pull Request**

Ideias de contribuição:
- 🎯 Melhorar detectores 360° com datasets reais
- 📊 Novas análises geoespaciais
- 🌍 Tradução para outros idiomas
- 📱 Responsividade mobile
- 🐛 Correção de bugs
```
