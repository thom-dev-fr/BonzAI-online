# Support BonzAI

Bienvenue sur la page de support BonzAI. Vous trouverez ici les réponses aux questions courantes et les ressources pour bien démarrer.

## À propos de BonzAI

BonzAI (BonzAI-online) est un assistant IA qui privilégie la confidentialité et fonctionne directement sur votre iPhone, iPad ou Mac. Discutez avec des modèles d'IA puissants localement sur votre appareil ou connectez-vous à des services IA externes.

## Premiers pas

1. **Téléchargez BonzAI** depuis l'App Store
2. **Choisissez votre modèle d'IA :**
   - Utilisez Apple Intelligence (intégré sur les appareils compatibles)
   - Téléchargez des modèles locaux pour une utilisation hors ligne
   - Connectez-vous à des APIs externes (OpenAI, Gemini, Mistral, etc.)
3. **Commencez à discuter** avec votre assistant IA

## Fonctionnalités principales

- 🤖 **Plusieurs fournisseurs d'IA** : Apple Intelligence, modèles locaux (llama.cpp), OpenAI, Google Gemini, Mistral, Anthropic Claude
- 🔒 **Confidentialité d'abord** : L'inférence locale garde vos données sur votre appareil
- 📱 **Multi-plateforme** : Fonctionne sur iPhone, iPad et Mac
- 🎨 **Interface moderne** : Design natif SwiftUI
- 🔧 **Personnalisable** : Ajustez la température, top-p, longueur de contexte, et plus
- 🧰 **Support des outils** : Recherche web, météo, localisation, et outils MCP extensibles

## Questions fréquentes

### Comment ajouter un modèle d'IA local ?

1. Allez dans **Réglages** → **Modèles disponibles**
2. Appuyez sur **Ajouter un modèle**
3. Sélectionnez un modèle dans le catalogue ou entrez une URL de modèle GGUF HuggingFace
4. Attendez la fin du téléchargement
5. Sélectionnez le modèle

### Pourquoi l'application demande-t-elle l'accès au réseau local ?

BonzAI utilise l'accès au réseau local pour deux raisons :

- **Traitement interne** : Le moteur d'inférence llama.cpp utilise un serveur HTTP local uniquement (127.0.0.1:8080) pour le traitement des modèles d'IA. Ce serveur n'est pas accessible depuis l'extérieur de votre appareil.
- **Services externes** (optionnel) : Si vous configurez des services d'IA externes comme Ollama ou LM Studio fonctionnant sur votre réseau local, l'application a besoin de l'autorisation pour s'y connecter.

Vos données ne quittent jamais votre appareil, sauf si vous choisissez explicitement d'utiliser des services cloud externes.

### Comment se connecter à des services d'IA externes ?

1. Allez dans **Réglages** → **Modèles disponibles**
2. Appuyez sur **Ajouter un modèle**
3. Sélectionnez votre fournisseur (OpenAI, Gemini, etc.)
4. Entrez votre clé API
5. Sélectionnez le modèle

### Mes données sont-elles privées ?

Oui ! BonzAI privilégie votre confidentialité :

- **Modèles locaux** : Tout le traitement se fait sur votre appareil. Aucune donnée n'est envoyée ailleurs.
- **Services externes** : Lorsque vous utilisez des APIs cloud, les données sont envoyées uniquement au fournisseur que vous avez sélectionné. BonzAI ne stocke ni ne collecte vos conversations.
- **Pas de suivi** : Nous ne suivons pas votre utilisation et ne collectons pas d'analyses sur vos conversations.

Consultez notre [Politique de confidentialité](privacy-policy-fr.html) pour tous les détails.

### Puis-je utiliser BonzAI hors ligne ?

Oui ! Lorsque vous utilisez des modèles locaux (llama.cpp) ou Apple Intelligence sur des appareils compatibles, BonzAI fonctionne complètement hors ligne.

### Quelles sont les configurations requises ?

- **iOS/iPadOS** : 26.0 ou ultérieur
- **macOS** : 26.0 ou ultérieur
- **Apple Intelligence** : Nécessite des appareils compatibles (iPhone 15 Pro ou ultérieur, Mac M1 ou ultérieur)
- **Modèles locaux** : Recommandé 4 Go+ de stockage libre et 8 Go+ de RAM

### Comment supprimer mes conversations ?

1. Allez dans **Historique**
2. Balayez vers la gauche sur une conversation (clic gauche sur macOS)
3. Sélectionnez **Supprimer**

Vous pouvez également supprimer toutes les données de l'application via Réglages iOS → BonzAI → Effacer les données.

### L'application ne répond pas ou plante. Que faire ?

1. **Forcez la fermeture** de l'application et redémarrez-la
2. **Vérifiez l'espace de stockage** : Les grands modèles nécessitent un espace disque important
3. **Mettez à jour** : Assurez-vous d'utiliser la dernière version de l'App Store
4. **Signalez le problème** : Contactez le support (voir ci-dessous)

## Contact & Support

### Support par email

Pour les problèmes techniques, demandes de fonctionnalités ou questions générales :
📧 **thomas.leconte.developer@gmail.com**

### Communauté

Rejoignez nos discussions communautaires :
💬 [GitHub Discussions](https://github.com/thom-dev-fr/BonzAI-online/discussions)

### Signalement de bugs

Signalez des bugs ou consultez les problèmes connus :
🐛 [GitHub Issues](https://github.com/thom-dev-fr/BonzAI-online/issues)

## Ressources supplémentaires

- [Politique de confidentialité](privacy-policy-fr.html)
- [Conditions d'utilisation](terms-fr.html)

---

**Besoin d'aide supplémentaire ?** N'hésitez pas à nous contacter par email ou via GitHub Discussions.

© 2025-2026 BonzAI - Thomas LECONTE
