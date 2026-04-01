# 🛰️ TerraLens AI v4.0
### Plataforma de Inteligência Artificial Geoespacial e Análise 360°

[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel)](https://terralens-ai.vercel.app)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/Version-4.0-blue?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-Beta-orange?style=for-the-badge)]()
[![ML/DL](https://img.shields.io/badge/ML%2FDL-40%2B%20Modelos-purple?style=for-the-badge)]()
[![CV](https://img.shields.io/badge/Computer%20Vision-Bounding%20Boxes-cyan?style=for-the-badge)]()
[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen?style=for-the-badge)]()

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
- ✅ **Bounding boxes** desenhados via Canvas API com cantos decorativos estilo profissional
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
Detecção 360°: Grid espectral + bounding boxes via Canvas API
Mapas:         LULC K-Means, NDVI RdYlGn, Falsa Cor BGR
Gráficos:      SVG puro (Gauge, Radar, Donut, Histograma RGB)
Deploy:        Vercel (CDN global, deploy automático via GitHub)
Repositório:   GitHub (integração automática com Vercel)
```

---

## 🚀 Como usar

1. Acesse [terralens-ai.vercel.app](https://terralens-ai.vercel.app)
2. Escolha o modo: **🛰️ Satélite/Drone** ou **🔄 Imagens 360°**
3. Filtre por categoria (Urbano, Ambiental, Agro, etc.)
4. Faça upload da imagem (PNG, JPG, TIFF, WebP)
5. Selecione o tipo de análise desejada
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

## 🤝 Como Contribuir

Contribuições são muito bem-vindas! Este é um projeto aberto e a comunidade pode ajudar a evoluir a plataforma.

### Passo a passo:

1. Faça um **Fork** do repositório
2. Crie uma branch para sua feature:
```bash
git checkout -b feature/MinhaFeature
```
3. Commit suas mudanças:
```bash
git commit -m 'Add: MinhaFeature'
```
4. Push para a branch:
```bash
git push origin feature/MinhaFeature
```
5. Abra um **Pull Request** descrevendo o que foi alterado

### 💡 Ideias de contribuição:

- 🎯 Melhorar detectores 360° com datasets reais e YOLOv8 treinado
- 📊 Adicionar novas análises geoespaciais
- 🌍 Suporte a imagens multiespectrais reais (Sentinel-2, Landsat)
- 📄 Export de relatório em PDF
- 🗺️ Georreferenciamento das detecções com coordenadas GPS
- 📱 Melhorar responsividade para mobile (PWA)
- 🌐 Tradução da interface para outros idiomas (EN, ES)
- 🐛 Correção de bugs e melhorias de performance
- 🧪 Testes automatizados
- 📚 Melhorias na documentação e exemplos

### 📋 Reportar bugs ou sugerir features:

Abra uma [Issue](https://github.com/flaviocaos/terralens-ai/issues) descrevendo:
- O que aconteceu
- O que era esperado
- Passos para reproduzir
- Print ou imagem de exemplo (se possível)

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
- [ ] App mobile PWA
- [ ] Suporte multilíngue (EN, ES)

---

## 📬 Contato

- 🐛 [Abrir uma Issue](https://github.com/flaviocaos/terralens-ai/issues)
- 💼 [LinkedIn — Flávio Silva](https://linkedin.com/in/flaviocaos)
- ⭐ Se gostou do projeto, deixe uma estrela no repositório — ajuda muito na visibilidade!

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE) — sinta-se livre para usar, modificar e distribuir, mantendo os créditos do autor.

---


</div>
