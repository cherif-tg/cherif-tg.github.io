---
layout: page
title: Système RAG
description: Pipeline d'ingestion intelligente avec LangChain & Gemini Embeddings
img: assets/img/rag_project.png
importance: 1
category: AI & LLMs
related_publications: false
---

## 🎯 Objectif du Projet

Construire un système **RAG (Retrieval-Augmented Generation)** complet from scratch,
capable de répondre à des questions en se basant sur une base de connaissances
personnalisée — plutôt que sur la mémoire figée d'un LLM.

---

## ⚙️ Architecture

Le système se décompose en deux grandes phases :

**Phase 1 — Pipeline d'Ingestion** ✅ *(Finalisée)*
- Chargement des documents sources
- Découpage intelligent en chunks
- taille de chunks predefinis
- Génération des embeddings avec `models/gemini-embedding-001`
- Stockage dans une base vectorielle

**Phase 2 — Retrieval & Génération** 🔄 *(En cours)*
- Vectorisation de la requête utilisateur
- Recherche sémantique dans la base vectorielle
- Injection du contexte dans le prompt
- Génération de la réponse par le LLM

---

## 🛠️ Stack Technique

| Composant | Technologie |
|-----------|-------------|
| Framework | LangChain (Python) |
| Embeddings | Google Gemini `models/gemini-embedding-001` |
| Langage | Python 3.11 |

---

## 📈 Statut

🔄 **En cours de développement** — Pipeline d'ingestion finalisée,
moteur de retrieval en cours de construction.

---

## 🔗 Liens

[![GitHub](https://img.shields.io/badge/GitHub-Voir%20le%20code-black?style=flat&logo=github)](https://github.com/cherif-tg)
```

---

## ✅ Ordre des modifications sur GitHub
```
1 → _config.yml          (paramètres principaux)
2 → _pages/about.md      (ta page d'accueil)
3 → _projects/rag_system.md  (ton projet RAG)
4 → Ajoute ta photo      (assets/img/prof_pic.jpg)
