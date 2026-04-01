# 🛰️ TerraLens AI v4.0
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
