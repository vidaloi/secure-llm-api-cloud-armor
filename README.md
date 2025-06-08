# secure-llm-api-cloud-armor
Création d’un framework open-source pour tester la robustesse des APIs LLM (Model Armor + GKE + Cloud Armor) dans un pipeline DevSecOps.
# Secure LLM API Cloud Armor

**Projet personnel — Sécurisation des APIs LLM en environnement Cloud Native**  
**Cloud Security | DevSecOps | AI Security**

## Objectif 

Ce projet a pour objectif de concevoir un framework permettant de tester la robustesse des APIs LLM (Large Language Models) face aux attaques adversariales, en s'appuyant sur :
- l'API **Model Armor** (protection des LLM),
- un déploiement cloud sécurisé via **GKE** (Google Kubernetes Engine),
- un Load Balancer protégé par **Google Cloud Armor**,
- un pipeline **CI/CD DevSecOps**.

## Cas d'usage

- Tester la résistance des APIs LLM contre :
  - Prompt Injection
  - Jailbreaking
  - Fuite de données sensibles
  - Toxicité
  - Violation de politique

- Proposer des **bonnes pratiques** pour sécuriser les workloads IA exposés en API publique.

## Architecture 

Client (Front React)
        |
        v
Google Cloud Load Balancer
        |
        v
Google Cloud Armor (WAF)
        |
        v
Google Kubernetes Engine (GKE)
        |
        v
LLM APIs (MitralAI, Hugging Face, Gemini, etc.)



